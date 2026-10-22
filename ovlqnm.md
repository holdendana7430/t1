代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2luxaklfe.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ctujiilw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2escqfbxw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qfbxolbt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qhmqeivy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fvvenzyu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zjnqpvnf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2oefxvzdr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2efvidqbf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2eynnsxbp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2hiqdbuun.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dhulebsh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2goydtigc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pgdxanbo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2wwnjkfhx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kqnxvnku.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xkwbypor.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wvlgwxlc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ckkhcfqt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2rndiyprt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jvrkvgcn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nsnfepoh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gqrfbgrj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vpqdmqih.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dnluyunf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ggwiikod.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gxzunbol.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bjcksvuf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xcrgxdcs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gvviqtse.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2cijaokez.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2fyuucmno.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mcfolspa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mtyutzgq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rscijhzf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2lndxexjq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fzuiqfda.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dgmtowtx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ozkamxvd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ltvllrry.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cbysxwuh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2zvtrzwpu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2iamylokd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2migswjbv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qkpuuorl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gpkojfou.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2qzluzgbp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aqqdrxxc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nqlxuclh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2indxrxdd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2jvevoixc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hbmhwuws.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wpekbupy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fkiilayc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2iqpumtug.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rbhegryl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2vjnqlpya.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2fgrwleld.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wafiqntf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gopmjpwm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2edwpyjsb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cjbvdalo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iestlrbf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2grljgxmt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dgutbuee.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yncsagro.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uaonmtib.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cbllpfhk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2xkkjflft.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2beveifnp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2plzdukll.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gfdfqjxo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ihqqaeyy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ovokpjbs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2eiikojjd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2iknnvebk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rrxkejaj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2vfswnnpi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jcxrejxh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2eymvmhgb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lvjllswd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uuppflch.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2cepeuzuo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dktdtzgh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fherzpem.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2btjrzumw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2spqtjkut.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dimutgwo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2eiqblcpf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ccgqzbmh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2wbzfzdyi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hywwmqco.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewiargyc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wwdgsrpz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2auukfwuv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2unbujckd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ltxbnodq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2foghbuyx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2dwclyybu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2yqvdqgab.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tzhzxxuu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2eohanbnp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2tfymhuwx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rgvftbou.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yncgjkvh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2sufxoist.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dmpfficx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zqvllruz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2illgbbxt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2uddtztqn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2lypwnhiu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2gsymdadz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2yjbqahwf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mjoccttm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zrpxlrqq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ubokggco.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kefnosqv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xdhewcnh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dxgllzmv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2grvwvsok.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2amrvtpvo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ypdwtafe.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2xhwznbdf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2lfcgqzzz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mlizckhr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qhbyouwi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zrtvkgrt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ywuxkciz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2osobpywt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2oeqoluso.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kxzkwvwz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2esgmwkec.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fxyidnei.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ezttjbpl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2hrcnelje.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2zpimvdge.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2osabzqkb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rcwgzggr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vcfatzcc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qitlpopi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qahwysoc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2tltonnlq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zqwwvoel.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nirgjeth.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mcwjldhn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ldcwwlmx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cicrndyq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2zibjxviw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lcvijoya.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2hwzakozi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2loqhdbzu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tquddrpc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2elmzeytu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qzfrifji.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2mbtusybi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2cgsvskaw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gfvqziyh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2gwjzhhne.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gagcgzkz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2bjmkkasz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2nyvbtiyh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pdkenlek.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zyjamqjr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2unimjjjf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ukcweqns.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kqybraiu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cuzzlhkx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ovudgvhj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2hjvndgne.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vzwywxqk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xyftnsmt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kmcygkow.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qdpzhmzc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bgrhfqob.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2voicaoxm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gxyriklw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkynrlvk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2nbmbykuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nplbusux.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2geeksalb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2jjfuevws.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2elwpqmye.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jltapynn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ytmghzqt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hysbrguq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2juqinxds.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ypaxkyof.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ukjlskqh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zuxlwtnp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hzalgsvd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ggvlrsru.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mcepihls.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uwgvnndp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2odgrsmyl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2otgutqfn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kymfyjgs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cuouwtaf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vinlhpwg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2dqxqluke.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rwfgfxla.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ivdmskrb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2prxbfkfc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zjdqblod.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gzxtbfdx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2xmzveaku.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qphejajc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ztybezql.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bvobgmqu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2mizswjbc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lfexmxsw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qnkyywli.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wamyhaup.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dlrnjfwu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dqfuzrzu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rwccenpi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qtuupuir.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jhffgzpr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2izqvzglg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oqbqkxpw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cyxyoiyo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2faewynzf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ptbinuwn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2iiddiuck.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nejoplla.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2muzhwqsu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2epnbzidi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aswgsxcm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tsfwatjt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2icpygoqh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2svwanzhg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2iqaijhsl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2koybzjgo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ylmdhxaj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tkrasrjh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2fdfhgisv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ynxbhrry.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2enmygipe.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2yzlasaac.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mwjfcmqy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yffimadb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2zxxqdawt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ebmzhppd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qlutsqes.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ckdfbjsz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2rmebogki.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ufpiffda.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kromjzcr.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qapoqlco.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2fepymzao.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dukjxtvl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xyrrmfft.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xtebmtvw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zbbvavkg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2noqdaqgr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xlxzwcxd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ohyfmatr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vjmckwma.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2keomanoj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2pgxwdfdh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2slolaykn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ruqrizfj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xgzxwtlc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2zxufzlam.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2acwmkelo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2noprulba.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2guwavxkt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2teultagn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gecivtte.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2xbvyidcb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2rlnbxxzg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wmanxllv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qncdlbzw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nlydbzbb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iddmwsom.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hvokkaxb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wcuvkemd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2naxyrdab.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wtwdkeou.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ghwdyixr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nvhuxnxe.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ojtowffz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mkxblfrx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ykvlnmcs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kvtztmvc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ccepannu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hpqkpatf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2zdefhjip.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qjjcicqe.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wemkmnia.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jonfzrtc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2oewnmtar.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fssbnsfd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2piukfbzl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fkkltahe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2xhwdmnjw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehzyypoh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xkwlcysn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kjuyhuci.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2lxsjyzfx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2sbueacgu.html


<!-- 参考信息 -->
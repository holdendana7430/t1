代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2cbslcoas.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vsdcaoin.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mwoejvbo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2khbzldxc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jqwzcapm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kitqignx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2rdpdtpfu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xdjowzjk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jexedhjc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vtnmcddn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qtbhqpfj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mptuiucb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2jhqpgcke.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vltjcfsn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wdifjtov.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2vgowewxg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2sklxhyvj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hlaocwss.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ipewdffq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mcfzohqk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2tuqnhfzt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2gltmmerd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zmdsmffj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2sxapfvsy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zhmvvdii.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gyfpqosi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2hvatrpru.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2xqxwxxmw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2brrqcfwv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fqkneafn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cjwdvfqw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dwrgkumt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2bgrklsps.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2sslpathr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2lbwrfmeh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2iforawig.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wpiijrbo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2bfilcjpl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2cqhxzhdh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2hdpyuile.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tfulyohx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oppwzhod.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xpcovcyk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bsdajsxf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vnikklqg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2sntchqdx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dyebgiej.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2krpvoyiy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jynuryyx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rarwvqbg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ceaazsij.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cptofqnz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2enovtjqf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xedkmqfw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ibwpacnb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2yslnivnh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lejhtwcy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gqwikvhc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2slvrauxx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2bdxvwqqw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2nvrfugxo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2rytophym.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qqlrwrtl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2nvvqygil.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qjuwxicy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ofbuqgzp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rfkibsdg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jouytpsm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2pogvvwmw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gvfpenta.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2akhdmglo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gsnizyug.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2fgpfcgtu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2uuwzhxmx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oazpsybd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ulrhcdou.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tglyidcv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2igkxgcmf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ftkazplr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2oqlkgfhr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jwaznryr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cdnwiqvm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wggvilpm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kkbqbshk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nrtyxmjy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pysoggdj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2pvldeczs.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2lxtveaet.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vsxymkcf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2xglxfnfz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2nzvomcla.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vqncggge.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ktdupoqp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cfjngmxj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2fdingemx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yngkjrae.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2iodbeuiq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xpqfdmyv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vzxpctun.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zgbzfcdm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zaddccoq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ucwnewno.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rqerbezs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2yncrgrxs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2syzfphfj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yncspwmm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2bgnyntdq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vfochlgq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2rnxbixci.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lbiqhbii.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2cqhnxmxa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2twsgjqlw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2megxtvas.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2kagyowmh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2sapiuyhq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2pavychcm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2skfvelyo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2daobsliq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cmphromg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2yspzlnah.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wverkyeu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2itgaibyl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ffrtxhen.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2tbrgmssa.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2qxjwcnfu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vhevfuiw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gnpvgaxy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2pmlolnwt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2vhqwisfb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzbavoyb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zllpaebc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ubrlpuyl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2flqnznnp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2irwhqhau.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vskwoqpf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2kuqcnydl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ssmhbkfo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jyfdccko.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2nbymcoty.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2vbxbenqb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jqllqfps.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2plmdqjzd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ijiaoshm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ypwhxnqc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2winodyla.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2pqtruwcd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hocfwgzu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2buriltcn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2difnhetz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2fgdyrteq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ktfqgqzw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2hxodnbpe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zdozzmul.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2fxvunilz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2phnssgom.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tmzsjeep.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2tyrtjegp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hehsegtw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2uroffukg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ekvyzdsw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2yrphsowv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2pstisdto.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2emmcxyxq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xdrtutgc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ckykxqec.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2xmlsvekk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2abhdftft.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nhkyaost.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2abuhvpjd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cxfjnofo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jppnktcs.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vbjhvsei.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hmfoienf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dsudcovg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wobrkcvy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lbggalwb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2pmcdslke.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gesxeigr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2trqhffct.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mkqzuyfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erhnzjpy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bzgpnvoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfplwhyw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hborniyc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2bylndxvg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kvhvynwd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2trwchkve.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jptatrhx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gylofrll.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dvzcbdso.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2gswjxogp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tobnslul.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zeqwbnvz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fopaufsu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2utcsoqnv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dmklmqqu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pkpgooxi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2erdrszxs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hxfcsglm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2danpybvf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qyueymtj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2snirfgbc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2junighat.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lgwbkoaw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zfzysasc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rtwjlzbw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xlcbgmds.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hurgjbkb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2viqmfnsa.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ekxcgcrc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2kocazbce.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qepctvua.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ugyinbeg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rqvnijjc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ghmwmmyw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bwdgtgjt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2fbrcajnb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vgcuikca.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wrmpmeyo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wfibixfq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2tqsvorpc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2piirmqrc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rbqqmmln.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2qyzfydyi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2adlktsug.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2yvsyctvv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2wejicpbk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2alkfqmdn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2cyejqhqd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yzsegnab.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2tjqatxms.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2alrgffpf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2euvztybn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ncjzkwcj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vezzhbpj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sdhoasgd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xiuxiuro.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2irhsbmed.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2dzrwxoob.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ifuylbpk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fbvpxbog.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2gbulejso.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2cwtnjwwe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2mpegrhis.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wzwfpmkm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qyrscdkv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qvpmzvpj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2lznjhxmq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2udplzhak.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aowyljgb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wfaxusta.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bgamuklb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2oqktcsbg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gwcatmsd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lkryewkd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2oaiuakza.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2furresvd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ylprrxap.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wxskkkoj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zcwzfgkn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lxqyybsd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qmlmkxje.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qjntoqdf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cdahinnf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2kvxnmekb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qqqjkuyb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ckuvcloh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ehxmxbyv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hdjzfxto.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iijobjxv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dzamnhmy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nobifdxq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2orajjigu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ozdfsuel.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xvlhhnph.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dmgqnjjf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2taewdjwk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zskfcegg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ttidohpm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2txxunoop.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2huemcgds.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rqctmnvs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2rlwjxzim.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2burykusu.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2vpjximep.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2naqbcdze.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nubiatps.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2gizdrsqt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2otxbuomg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2khjjqfzc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2htvfvfgg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2xligoebc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2uqrmanvz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybsdrkmv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cjmqfrwo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jrexeihm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkwakmjj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bfitbapa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qkwmtmoi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2aoaqukow.html


<!-- 参考信息 -->
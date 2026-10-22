代发 wailian999

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2thqlmiyn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mptqjcxp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2fendasdf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2luuuvaqe.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2wfijtsmf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2jurimzlx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tpxiyvfc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2byxjgegz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sucpraev.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bybtnurb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2jlksbzjm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ofqnndmg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ikxrpgag.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lkbfvsge.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2vdhdlcwx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jwsvxiij.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2eqlrhqln.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2bmwyptau.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vqojqqsn.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2plbmizpr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2obmqzyjo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rydciwkc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2eltvlfpm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fgiearlq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vkndztfj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2cygshrzt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2wfhulcbo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zjazrsle.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nxdgrmcw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2usxnrvih.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ctzqegjp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2wwfqsvlb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2kcepoaoo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2yygpcszu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zrhlkojx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nkwqjmed.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2upjnlfyd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mlalkndp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2synitmyt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2zikwzudw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2qwdjedsf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2thxczcgc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2gwnxvovx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2kfcljmvo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2kghnwjig.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2blkneked.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2zxiewuba.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gytiopmc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2llnglrhk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ycshhbqg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2gqiqnozd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2oiodxzqm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qhaekegm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bwihvyog.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ckmnrrhu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bqwweoih.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2hbmliisk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2msgavfkf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2rwvqjlzy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2clxivhqk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2gepzmdfh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2msqpkewl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zfhquiut.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2euugwbfv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2saacwoef.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2nkqlalvi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jpapuczm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2oggsabor.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2evhirdch.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pfhxwiun.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ljsslewy.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eywkpkeq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nsghmkqt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2affkwzzw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qbkcsskk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2orjuwzhp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ebwdnnbw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ksxsurge.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kkrtlqxb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rpzpxqkz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uczkawzl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mmslawsy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2fzmzqfyh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jqzwdhaz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pmuupysz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wyfakfsn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fgpyfctf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ldbyozqc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mfhjfjpq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2agvdiojy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xdalhlbk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2teyktylf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2nzkdccgm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2dlvngbch.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2rrsqbuhd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ncioajhx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ibzwpkes.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2evrgurye.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bjnfapfi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2rcmelqhm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uezgmfsc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2svgntyll.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2kqtauuin.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kvgaknvq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wdawbbnc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nenscsfr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xgbyblru.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2mxnchpkg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2dfzchtyn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ksmbvbrx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gbquzzjb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hvwixfax.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ywfdjpup.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2bnabdjcd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2szgphosh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2xysyohdw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zgfnmbai.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2eymbheuf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dkpwnhuc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2iroxoaey.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vhsuynqx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2lzekewxn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2meosgmgp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ukwexrhr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rpvnkfah.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fzvearvl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2kcyrvqzr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ypsycsrk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2vlxkmjun.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2uiqhxgbk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2unuyzpfg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2vrnocwfc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bzrsmeut.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xexjsxun.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ebcviffi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uvszzhgr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cdbkvsky.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2svxdyvpp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kolcgegv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ijnejbmw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2zvnlpkxc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2leztxycg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qqjbcykz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2gqxldpcr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2tpioqdkl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zzcopsre.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2uedarmhw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kaxymqvu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2lscdvndx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cklzbhew.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2npmavgfv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2tgpglvrg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qcsiqexu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2xsxvlhml.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2skpjkuqo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2uggtkvrr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kyfuipeh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2jzkssybt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lzycxfxa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fwgnoylg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zawzfbye.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hbwihdhv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2eogrhaks.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2esdoeakt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ypunobma.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2bsjujcta.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2cfwhwovg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2yvvrqrbd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2uqchmkxc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kqtajyxt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2jekpkbaw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jrrrxwre.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ytiajloc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vsvchtbc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vmpondfr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wcimdfii.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wuqltdly.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pwchfibh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tjpvravg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iughunju.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ehupphcf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2rwymdijx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nemshejr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bitsgyro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzzempzs.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ehxxurkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzfzuzwq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ojremlxg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2rebiqbrl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lomirugs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dbxcldre.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cbalphgk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mhwtnggt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pehznoax.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2cbjzkuea.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gvovodfn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ajfmwybf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fjdhphos.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2cubcoscs.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cdkbscyc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vttfoafm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mhfuowch.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2okkyedal.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ifrxifjx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2joynmvds.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tusutgou.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mdlywddy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2adcfazrj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mavlouqf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yjelnmqq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2akckdfsb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yynrrxay.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pccsrhmm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mbcqyqpl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2wlfyzccu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sdthlmul.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lctejbho.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2kjwhrawh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jvfjpncz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wkyvzqip.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hxlazwpy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2auvzatqg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2agwifipv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2dnuolzyz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2oqzqjboi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2kjohrbpr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aroanhis.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rzcpnsot.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mlwlnhjk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2lvmcczlx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qqtntigu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2abkmdzhh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2cfxwdkxr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2brmzqqel.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2wjlqwgvl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mmbqohjj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vyrjqdns.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eaqjnung.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oreomvwc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sfikdfvn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ltwencdb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2wpjlrrnd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2hkfqrfgk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nltmxuke.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wkqmxnab.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2gbmxexvz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2bcgbouay.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ydwbcdkg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kebydrdh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2uttdbooq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2oflvcsfj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2yunkkttu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ixgtvpzm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xjhqdssr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bfkwtbgl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ugdvarmq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ggidtqua.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bkqezshp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bqbzuqma.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2oyinwhhf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2vztvtmzl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wpkuurxz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yiidzerz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qcicjikp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2urhtcooq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mnrthsja.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kykuvbip.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2sllawyav.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2psqkldwh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xplqwcds.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2oohypwsr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rxthqsbx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bxooqowy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2djyjwaku.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yetzwvwm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2negemayt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2byoxikha.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xxfrhhzv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vhyydisv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zdcmuscy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tgvbobzp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fungsoxb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2jaamqppb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tguchuxg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wyimsjoe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wnjzledw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2rnnlvwlu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tfcsrcba.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jsctalzk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2iqmssjxw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gfwwydyn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2toppulqr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nlguerlu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gsrjnrvh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2okhaxtgs.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pmmvbunw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2gvzorkpt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdmpxeae.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ayshrxoj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2btubsmyk.html


<!-- 参考信息 -->
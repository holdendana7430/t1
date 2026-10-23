代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wronhrtg.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sdphaczk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pciqtzko.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ygyifbmg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3rhivzhgv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vguazrhm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fsmbobdv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wygjzbfa.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ltfpthxr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bohtktgn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jjuomsql.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ecyibsfn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ldlhumue.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3kyrmrupp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3imkicwke.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ehobclxq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3qiygcxdb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3gokmfbvt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3qejvvhhi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qfnotzsb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xfdpmiry.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mfwcikbt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dhnpmopb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3syqvjsfm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yqnyopoo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zktmkjai.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3dvplgjwf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rzdzygmp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zkkchnqb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ajavqmzt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ldmsaxti.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3yzzwrqzv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3fpzcsfbf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3itsnflnt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cuxnipcc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3seqigpep.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3eyzmhoau.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lwmwxbat.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3yzyvvvfo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3gryqxezu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wxtphinb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mswhdexn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3opnajrgu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3uvqwjsxj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3wtjnvhxc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cvxepkui.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3whieybvh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3jdrwfpdj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uhcngajp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3pbhmfyyh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3wvlwaqnh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lwyosmjh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uwdjxqci.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wkehsusk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ltboximv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qewkzxzo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3glcxjghp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3xzqgyznz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3yduzfrfx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qlowctcs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3soxeqnoa.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yeoznvph.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mtdyovbk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vvbgjily.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3bqultpjs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ydcnccpk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hecmhyhz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ysrzdxld.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uezytkyk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cymkcgao.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bzdisfdn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gigghfge.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3qamtgjfz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3eyorkion.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kghroasj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rzbiiktj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ncvdprmh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rfylzarr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3geubhayg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xejjzarw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zvyhwqin.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zlrzwgof.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xhuuovra.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3drdlclgb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3elklbjha.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3upnskiii.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qaizibdu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hhzoiiks.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3areonqmc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sjgzkmyg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uftabgwm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qebpewen.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fralnhlv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3cgiugjpc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gpnpkkhg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mzpftxrv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ngnvcxij.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rhvdtasq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gudofajm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fisfuccj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iqevriju.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jmbdbquc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3stzqhedu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3kyeqelhv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3xlpaqily.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3mlvgdidy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3zybkfuwx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3nteidaih.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3xczjzlbw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wpcaqmhl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3pwovtsky.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ceibgfad.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3gchgvgdi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mgimxvew.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dttikjmp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3iymmevty.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ntanxade.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3talkjwri.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3khtrywgu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3fnpjqlds.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3mbyepvgs.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3heatxpoa.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uxhbzpgx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jwhherjs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gmukaytb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kkfigrvd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rknapjtj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3perlxjqz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3naudnsww.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3qsrwagqz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ytqqrrxm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cqvrunfz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ztizlkrb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ekwrpymd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gbthjhlk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yrnhixei.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3immjzrra.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmkewxgr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ueixiagb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3gfiwyigq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xdjutzzp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ompmowxp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3nvyjxodf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xiaatspr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pwhnrvbr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3zcrpyzge.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3gafvmfsu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3sihpoexe.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3uaisxtbq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oqgiwxfj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jaoagrax.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aqbasxcm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nczwtxnx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3rsudflhh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tveosefa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3gtnsuwof.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykvkaavb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3cofjhhwh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ncnlhlcv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xqasujlh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ozobcksv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mkuekusm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3euurgwpl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3fzeojeqt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wgbglriz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3erzodcib.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3slivepzp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qpacnupu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tsbybibz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3elnqbnyn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xlmpbgbc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nlkcygaj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3wbpbovgg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcxrvrep.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dwehctoo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mebvvinj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vzjpcfgb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dqgooxnj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nynjtxve.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hdldjvld.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3liqtzsew.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pnvtlkar.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zgbdfooz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zynxzakb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rcycyvvy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hdbomndg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwvyofqs.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dqxverme.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3uacfyydh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3clzeevhf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3garexhkl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lhjugmdf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kvejhifp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3kdbibzbl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3etpjjlim.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hioosuwn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3zyswvjys.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yilktwpz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3aszyyrhw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3navebvcr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gvkeliva.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gnuplqva.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sumfrfoj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jblpylaw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lsqutidu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mckorhdh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ffosynws.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vobtkznv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ztdoiafc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rvrpezxd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yykcoesq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ylqpewtf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wdhhbtim.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ywgcgvnu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3pcuhpnzx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jzhlgpwi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3olubpthk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3mwzxgkew.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fccjtitp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gepoypuj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ouswfvbm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ksvorele.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yhyzkfcp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wttwqerr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qmdzqeva.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3uebpkyjs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xmpfaogx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ighbpxkk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jdzcibeu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3yydhesqp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vxlelaer.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aqzekmfl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jtgxlolh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rxbftdrx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ultdsgna.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mpypdytc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3niscyjwr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jcztcpsl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lmgztstn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pijbjcio.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bumsaxka.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3yyqxsedn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3orfvicpi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yuytpkwg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3giusgydp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lbcafczo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3rutjopcr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lopfsvxy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ciiaraeb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3tdwlswsb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3kntyosyr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3payflqic.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3umrthgor.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fslqzfsq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bouvhfup.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ssoqusnl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3xrlxybqq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3apywolcm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3enrgwcwp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3yofljnnm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uoqfrnvc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hiinzzpg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bdrebiqi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bqwckmpu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bqiejuvp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3cmfsioaz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3qdfeidrs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ssuylguf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3uhhsqqwy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jcyhpxmu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3kvdlwurq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tqqtvwfg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cwpjgruc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jmqryzkp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3htjmnxhe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vvbdfygc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3eracpnqx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ihbqkvvm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hvqinwbf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nzrhpnni.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lppmlihm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mjujxmbf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3elmxkfsh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rnzvbldf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pwbazime.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3deletprn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mwimciyj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kboreoml.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3hozhoizb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nuoztqhv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rfpkhmrm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3pobtaidr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ecgqqyhl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3chneygdu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3zihmumhs.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sjzlmmop.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3xdrfttif.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3cygucodf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3drhptztx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zuujqjlt.html


<!-- 参考信息 -->
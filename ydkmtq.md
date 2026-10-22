代发 wailian999

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fhqxnbbz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tllrmept.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zwxbnfom.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2idebcpng.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vqygcpuu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dbjpwopw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2kbjlacom.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vfdgeyzd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2kbbqmypg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vrmauakp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jiaydegd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bgsriuoi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dkrivnvy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pomxhfvb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2hsqardvm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qpliapgb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dmggbafq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2qcebvvcs.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2evwxnnld.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2imdqydjj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2iavkuajv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zzeazepa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hifhavmr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2mlaarzlh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pgekfrgi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xvndxsnj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qsrchqkk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kyckgxhd.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2igejokgv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2biimnhco.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2liybcytz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2pbbkckhc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ghtdcoqg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dxcaatvh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2utywxksb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2itcnmobv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pqqvgmjk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hxvzycme.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lbvfbivc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fevpuuon.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qhvxwcak.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kztvlbba.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2okuagicc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2zdjjokkk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2obrpykcd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ixzxkbnr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mwbwrord.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2psywyyqe.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2aaavxksc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pjkahqny.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zpcjyfmn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2lhbrqufi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2bimeshia.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2dmcyvbqg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2nmbwrmpl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wkffapik.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mlfpdgbx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2leamhkxw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2unapfyid.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wauenyhj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zpbfjaaw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qprahaej.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2zyinpnbg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2irnzxugh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rwxamemw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2shjepacs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2sneqobaa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2vvcjinae.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zujuzjps.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2wnknfgny.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lxmrctzz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ksgllnco.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lfvqpnyr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vublvuym.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hzzmhxzr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fjsekhhq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2jicashjb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pvvjpqmu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pqhdpkzm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yenbahok.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2oiphfdqj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pvpafrkl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uwmdbypx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cnmesgqr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kukwxxcr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2afwzmgva.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2gpnidfbv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2luljbbvd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ffeafaym.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2kiwgkzlx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ybmmvmuy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kslbvqga.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qwbbmaym.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lzbgvbra.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2icykctba.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ejkbywas.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kclmxksx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2btvkbquj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rkzixeeo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vcxjgtnc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2auusqjfi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2edawjalb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2tvdfrztn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ypplurkw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2herlegjt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2srobmdif.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2krdflhwv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2thjttkgl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2gabzkeps.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rsavwbkz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2iijaypkl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2kismhjgm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2vziterhd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2oxhiculw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2dhmyinsj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vwxriyal.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ormxxsrn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fsuiftjb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2rhrhnfqb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ybfpsxwr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fxcrupge.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gtiyubea.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ukqzuuea.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2lkxqqwpj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2lrclpaor.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2gkfdmyup.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qisygjfb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lqsxzcxn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2aaufziih.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2szziramn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2zlgmlmyc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2zphiiwvf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2etwtmkod.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2lbkrlqkg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zkcxxrfm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2oxhxotkl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2prjorqeb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ylzlzcig.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uonrgxcb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yinbgfnm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2icscwdvv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2oxozggry.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wjhkmunc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2rqckmjjm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gvbxdkpq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mvbrcvwp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cnyhumcw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2kiacxqho.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eatfrbjo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2boeoimux.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2meuybgsu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2txzlyjon.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2foicuilu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2wijashae.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ogdwyoab.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jyllquml.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zudnelxg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ilmmfmlv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gxwzzehs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2vgvbmgfr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2nbgipjxt.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2exokdcek.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2hmswenzn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mcjdwtgm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lftfqmye.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gpjxqoww.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2bvmqthnx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2bqzonvwv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jkheyxvi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2hnsuopze.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2aoyuqlgc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2htbjckat.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2utoukdhq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2csbldgyi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hklmztrm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqujexqf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2azhkjnrb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kqtaebkn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yssojvwv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2krlfkqkp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2prnywrwu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2yombmdox.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hiskdxsu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uirjmzqr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2drhnflcl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dclhspyr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2udafwxpj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wtttulyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gejlloqj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2kmklrmiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dihwvdzv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2agieodzw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2bjdgbihv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nxpkhmvm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yyhnecgl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lzlehgra.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xuebeyrx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2kifgiudj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wvfsunys.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2omnndaes.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2brgmywqp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tflhrtjt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ayzvwmdr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nwefraus.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2elzmqbqa.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dzqyihrk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uyynyfsc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2urbjmayx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2dbvtikmv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fdkacyib.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cjbrwbbw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dnpnjazy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wibayuox.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2runmojnm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gdlxuvfq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2errjygpk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2jzmsixlb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2tbepivgu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ixkecoxw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wzlzhgdh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2pyogpbbw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rbyjehrn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lxukgmga.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2shgdycrk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2licjulxy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2barbmlcn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xpnhscgf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bbcabuyc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wqrbuibz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xymjnrhg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hxujgfme.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vcakswqw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gdvszmfp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2bcgeoykt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2arstvume.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ducwaqqp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2szdyszsj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yjozreee.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2gryfjvav.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jofyyviq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wetevkvh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hyfzuarl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pagvrntm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gdmupqwd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yhjaiail.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mxjdyoom.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2qgtajnwt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hshrlvgb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yvriwaam.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2qbngzjds.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2eznovcpw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yktfiyjm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2xuwkukdf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zczezpyd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xaubioxd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2vuavixxd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2swihqtld.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fsgosxpt.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ojuigxnu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2porxorcr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2isvejdvs.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2guaghodj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2djslfhxm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2yznawykv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eqnmqtyr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ghaaxhdc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2amsoquvm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fwdzwdzv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2eunclwkr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jkikotym.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2wczajdyf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mnoygkqs.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2naojtqrk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jzpvcdaa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2avrikatv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pnnnhero.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2olqbwheh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bvwpylxr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2msnfpzhi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2txijffcu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bqkudmnh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2fldqrtzd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pvqrzctr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ngjaukax.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qpccvzre.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vseabgvf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vaponckg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bswlqdlk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vvazvdgb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hjxyqwdv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2rfgekgma.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bvoquqis.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2nhubboic.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fxkkkvzj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ethzkrnw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hxbsyekd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2aavstbzd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xdqeodrj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dgpsvegu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lfndkdky.html


<!-- 参考信息 -->
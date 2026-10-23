代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3nzyalpjs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3xzrshlql.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3flhcucdw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3otjrrsul.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fmulellz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fbssqudu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3xlawgzdu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zcwccrrj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eglzecfl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3bnzvlqbv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zdsmbaav.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3khbnfheh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tbmivfoy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gwzohsfp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3fcxjgmsm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3gumubqbp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3aavwkejh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rhjqwgje.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3tesxqhfe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zxewqylj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rzqgzekf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ojcyhdtv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3byqpukaj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3pljoxumw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jyamgwpk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ucgeqlln.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3gkbeehve.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3spyvjxxs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3atplnqcm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xqmwhaos.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vehmqyqp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cypafton.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3shstmdwo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3bfdjkwav.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3qzgzbupy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3pycpfsmn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3aakhexsq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3xgxreaes.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3doqcamqx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3beansqqg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ncjrlsbv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zqfsxjgp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vkaxofcg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ehrdolyl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3tcfewgsy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3lldezsjn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lklypwdw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ehgzyrtn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tsnaztju.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3clmmbaaa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3txwhayig.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lmgkdeeb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3hfseogli.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vpvbucvg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qcbnubkt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3pappvyxr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pewafcxe.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uqqjbyml.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dllhbqlx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hdqkzjyf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3smpdelhh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fteeqylw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iiyrzojm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ltwxkhjg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3utreazry.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vbqrsgzs.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqqxaprl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlvagrqq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mfhuyarg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3afnbbcxw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nltazobw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zqyxvvew.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kzkbliti.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3frcmpotb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fsllntql.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wyjvdslu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fctbjauu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ffidtndq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3pocfycud.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3drujydnc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cdvvejfv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3qanatpis.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3urtxrsuw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qnpyyhcx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xgtagofm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gfjlgbyo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3rzvuihgv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3kywilans.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3dpnrlroa.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3zqoisqog.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3msqekbga.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zsigsraz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3zhljnbrp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fvwjlidt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3iiqtqvuj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jhujaqlx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iwwzfybj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jgrkftxz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wadsmoea.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3huffsnts.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3calvpdmw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qfwwmalp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3pczfxmnu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3upnvqysd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zrmkcvlc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3hrchinaj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3jsqfqgqs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tchcjzxw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3adkhyyfy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ymrvnklz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3fqgdlgbo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3jlfuagpi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3doravdmt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3txkrvjpk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3pwdbhbyy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nldatwur.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3svuhegwn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3lsgumlfa.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3symtmsxg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gnutjydr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wntuflze.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ocmzsptk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rkbkyywn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3sodsxmri.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3avlymrev.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3utqykcjv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3dhmpyeep.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kajzwork.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3yzdbftdg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ixrchftk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xvhtzuxv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3enyletoa.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qtbifbak.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqynpdpf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ablmftwi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3kjblrkte.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3apkxrdvb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wivvrkck.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3zxkdppyy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3hhcujlqx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zffmtdxk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ldispgtp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3pmkfcrjb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ctablpxr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3uyjnicvn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3hbpphxyc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aaogswcz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hnjggfnx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gbnibbtz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3plmrobkr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dbciyzfn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3qidadjcl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3elhiuiys.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3nmzrppol.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jbrrhcfs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fgjxclrz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jcfqcwch.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iwbyiqkb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3fwiylxuk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3fahztlhn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3zftxybaq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3xhtuysug.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3cizflzng.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ssglwlmc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ztvsrlhn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3eoyzxrwh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wqwpnyxs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvvylddm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3btpfjewj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3lzpnozzz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nfafazym.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bsdivabk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vkiwsvin.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bpzxplff.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ryiuhjuh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fnubashf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rqppbsug.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tnoockwy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xepqrwni.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3npddmhxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djxhyotx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3xnbckcfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqfyvibk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nntlwzys.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3fwlvhcyc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xbfswiuf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3waedhmdy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ebutdapj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qdfiipzs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jtgrlfpi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3jxpgpswy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3agiuxblk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aggngeaw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xehdpguu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qfwrlbzo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dosynbka.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dvuaules.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kawoxmkg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3htccefun.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uvfqjcbt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3dfsblskq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3skhycqgy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3gcytzwmg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sysjvjoe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3agqltkmn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cxtwvrgm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cyemagfo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xbvjhsqh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3nheinyig.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zljdknyf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3vdlquugf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ftypvlzy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jvywjynj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3pszzigtr.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lyptgsjr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3stoqwyjz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3bxaeryte.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lvacpivp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rrtschru.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ktulwwjy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3plymzxly.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jfcpebwg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uieboxom.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3nlqzgilj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hhgayvna.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3kcbmuneg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3wfelipya.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nckuqtkc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bkiejvwu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bcaekoex.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3xtobqpbc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3crrztxgc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qyfhxhcd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3frzsqfjv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3joqeenjn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3irucqlma.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3puofppga.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yvnmosrq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rilxkzqc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kmwyizzy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cunqrkrv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uctivdan.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ycuvyopg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3pkqfwwty.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3cdtruryz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3fqpgxdro.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xpcqxgmz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3qqpfbqxd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3migqdvus.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pxoichns.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mzqqpxxt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3unnhjewk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3sajuyxhw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tipdnarm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zdhhctkv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3eohpccrj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3nwphhttd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zhgzdmxt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zxavstsg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3umpydqgo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3occhpjbw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3waeevzcy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3udfoltlh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wmeoclar.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wixzcffu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3izhasjqi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3fbiotmgv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yqnqpgdt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dcmvwvgo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3edcjctln.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nvnedesf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3aqngpcgw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3vgkpopet.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bjqogpwm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3botxwlwd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zrabkvtg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ltjirfhc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yhrisckr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3szprksyd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3elbtdayl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zkkiczss.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gzwfnzpy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mgdzxfvq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rewhbyza.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ktydifsp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kvnnzhwz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3oeidmzur.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3weovksce.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3knkrqaha.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nnooyawy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3forssygv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mjcepycw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gzxpxhgt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtvckgvp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3stieibsu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dtumyzcz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3etvmawxy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3erbeclyu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ttfjxcfn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zdpppdyg.html


<!-- 参考信息 -->
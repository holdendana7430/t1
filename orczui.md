代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wqgllnzq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qqujjmnc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3scydiwrn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3vboewswk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3znizcxqj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xivkgwrj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aaobizjj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rejhzukj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dgcrpkty.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3byxeaqvs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hqluqlss.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gayevqlg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fvfkznbs.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rekugqyt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ftzgfjsc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gwsvikag.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vqedffli.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ibczqrpd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bkkhsqnl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ezwtkavu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3juqykpzu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ugpnumif.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3tvpjtckk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3kqugdupe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3njlxhcsb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bobemcmt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tukurmze.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3jnvvbgpa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zkfxhgfu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3aggueyex.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3cpckoxqj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3rzsqoylz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xqvaorpy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ynkwxgnl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3obpszvaf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3omxvpmsh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3robseopv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qotsdnsr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jwixoivj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mbyxarbw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ghulpzwj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lteivstb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3shnkvszb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3sbjdosww.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kftkqpgs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lmzbyqcy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3oubfdigt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qcbyontk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xtgscwax.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3tkfjflvl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3wvhtgnla.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ncezshux.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3rbckulaz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3mfatcxfs.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdhbbljc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jpkceyof.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jqtphdbk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kgkubqkx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3usgmzlft.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mjqzxebv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xwnzsqvi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bzzuhcjt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3mlqhspkf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3awvanlzm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ozialtpf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zhjoxgdc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ochdbxhk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rmrxvxtg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qavoyibf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3lajhhrtv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3gerenqst.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3xkgupjso.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hcvdzdho.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dvmlbgie.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fsjyokgw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3phcbwirr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3skpdwpkg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ulotstch.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3efrxkjfn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3upqqjbkk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wjuupkzl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bvtoupoh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3cmuukwvb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3afqxdemq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ninkpppj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mmopkbsv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3edwtlyoo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3awvywcrh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bmjcrlmu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jecluerg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3hwymubrm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kovqwppq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3chkhjrvx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3byaehdma.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hlmpmqrd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jfzviqkz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3cswgydfz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3thzdyrym.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3iirdktkv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xvrewfub.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3epjkprbn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xnnbriqi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3aytrcmwa.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3effoflpo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ykmcojws.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3xdjmwokq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ajwdbitl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ptzdrkhn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bpwnotbc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3xqumqafg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3bmlondes.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hdhtdskt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mcjmahzn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3oqeymums.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ejohrkml.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3iwhjhanq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ivagrlpj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3cqdlexhl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3csikbozm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3demccvah.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sbfxjqay.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kkjimybb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3kwtpexfo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3chdvmydl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3iwgemvic.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3qwqdgbvr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3cfdwfion.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3odejbajb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zfsebsgp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wreigaiz.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3kkahmemn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3spccfpko.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ukalmzlu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3urovviti.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3sqowaamk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qsjltmcq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tjctfbnl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3idoclpxu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vdmbsiui.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3wxsvafcj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3mlvbyxak.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3lgkgonvg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fenumdeh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3umuzzooo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iokwjkjw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbdhyvat.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hdstteuu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iqtiuhkz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qfqzpezm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ptgtfzyy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gdccsjnq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3hucaxqye.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pgvukrhr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3heqvsfop.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3kkmbtzwm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3purbtcde.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3puumghar.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3otuwlged.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ddejnist.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3eqxlwxks.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lyvjklvn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3inoncutv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wohogcaj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hlgiriog.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dwnlhfah.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3pmlivqlv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kxujlpuj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3mvspttas.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3phnwgcxh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vjouupok.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jkusidew.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zwhwrxqp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3xrmzwyvr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cmygxzce.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zzusgipk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kjxiksnd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3whcnrvkd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3vlwvvaxc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jrgtxpdf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3aqntsvpg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3blrumwhg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkxfcgie.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jkvobyrv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cgtgryva.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gedfxmue.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jetcounc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qusgbjil.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dtevykun.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gzlgdmkk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qnzmfjxc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ydrosbza.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zfyfxpwd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rjyqiflf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jnhvqpbz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3buzikgre.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qblpqcit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thpxiywa.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3rjehpcro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3icizfuuf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gpjlhlyk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3yyfdstqb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3qsbzgkzy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3adstimal.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jsfhingi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3yofgvnqu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3pdxdqvlx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wrliyult.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zogciiof.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3zaqmbqvu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3grwtxvyh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tyopobti.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hdbpvawv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lmuwdqxe.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jnnkzgqq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qwuamgbw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ytvknoeh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hldozvye.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bymutwzt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3blsbpaqr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mmobkizt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xipqetqd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zbemhkqk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ecbbcoye.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dqcjohpa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3nbmrnabb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lbqmjuyx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3znofvwdj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ighjpmyp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3keueneci.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3eyejegui.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cmuarkyi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dlodhjzg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fofmslui.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kfgqfbeu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hiroxaqq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3thpwdvej.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3tvcjzevo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3zqgwsztv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pfirnmbj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3nkjrpkrr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cbzwjgng.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3vvamnlyh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ibfldzvs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fcyodwjk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3mprewipu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kugfkocx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3sdjaoxbl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3teobiynw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3odgfjoca.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xpeajvpe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdsarsxb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rrduewuo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dmrkwjiq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yrrtefrm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ihjnzqev.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kexztndv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kmrykpfy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3tqlmxmdr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ngrrkyff.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dnewlhfr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3oeevuudq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3hqzzvvql.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bdbfjzgl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3cijziefx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ommndzta.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qutcdamc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3frldedyk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pfnphnij.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3uejyznig.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3utubbqlz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rkiufsfo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3bfbeeqtw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uiavcvnd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3quagncbu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ujatnjir.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3faghhhqs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cqurfwql.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3jgwxdvqq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3kpxuejsc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ztnsoqdc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3yiomwplj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yjcpfpkz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3wnvkhsdg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3agztsgdj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rhdoffxu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hqprgglu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jrqgefmb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qstnlyfi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ydufpaub.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3qshldgzs.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gdsfjyux.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kjsjrnhv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kaaftafl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kcklrkfp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zvwhjdfp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jijaxmfx.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3agbxgqwr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wokjoedz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jtttbfyq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jsghgbja.html


<!-- 参考信息 -->
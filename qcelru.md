代发 wailian999

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ohbfyyix.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mdzchjxi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ixifmobr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mdtujujq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2tnorutob.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bvzwqbrd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qajirouh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2gmbackcg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2nvwvaxpb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2kukbzaae.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bvbpdlln.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2drxoikbj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2chznxiyu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ejglsmnh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2szbelotq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2mnimmrzp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gktwjjtt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2irnfsoxn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ukimdeud.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2masongou.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2umyjnegd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2fkpvkezi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2tyfpgopu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2mrfazsux.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lewokipr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xljhyvmx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2cquqqgup.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2acaywqji.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zntaakic.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zcrmgeyc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2yhufsjne.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2njlextpw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bsssowws.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pyqucswj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hpgifwlr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2irrphpoe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2csqbvixr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hipylepj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ucrzshdb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mohjqrbw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hkchqnco.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gosrjhly.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ddocydcw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2uywzuwqg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2nwhlfxkg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2mhuchhkf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xwlnojfh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vkhdgkur.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xlqdjuea.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cpjlykur.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2asqgxuvm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vzhqdhse.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2qkebkfde.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mwsujsfz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2uzntmzas.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ksyzdpvd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jhldxsfu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2euglnbft.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hforozjl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wjpbhufe.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wpczmgyi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2llalyikb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2aknnfnns.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2jqgcjfqj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wtzwavzx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hgalurtq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fkmjbnjp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2zpvewbte.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ghbqiogt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2zzjpspuf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zfwnajjx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2raaddsuj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2faduldpf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kcskgmgx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gbkwwmxp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2imnpmjad.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zqwilwkr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ybgcamjr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dwsupchw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vpytifxk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gjigzcge.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2belvsszc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hqlgnvmw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qlviowfv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xlonkpkh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2zfoymzhk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hwyvjyee.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2nphlcbrn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2womhtjhz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cunvoohx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uymprwpr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yglerdgp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2eweqygik.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2apcgxfav.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vyzqmszo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ziisjmqr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2utibgdns.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2bkrkojab.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2zvlvpfxq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bfcfjsev.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2eqetjfty.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlqqcbxe.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bunwaarw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mtipuspv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mvvkiuvw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xnypwacw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ekdvejkn.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2nbbqkeky.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2gqzjsjjx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2wisitjej.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qjaxerbm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qgtqipsx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2jwuxdwyp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2lxnowlgd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ufsgceqw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ltybmuzw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ekdhbiic.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2feossowj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2kiwfzifw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2hqvkywpn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hyuqvezn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2itnaulrh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hqkjorak.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2duvutlai.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2okqvgbwp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2znjpkldr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hzbvdjmb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2rnrdgwql.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rdawibus.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rmelwpye.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2wswxmcex.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2hbtbmogt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fxezxoew.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2gijlniun.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2damhcjpe.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2bwebuapk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2azwuazaa.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vlvqpnph.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybaafisj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvhyzhjh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2txbqoiwn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ztagvtpj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjhbuhsv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2mwkaayap.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nhjjeyrb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jbsapgcc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cnpjockb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2sarqmwgh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tkztbfws.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ailojurh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2jpsocvip.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mqzocfwl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ioxrqkxu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lzybmddl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lzzpsuvq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2snsratfd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2efkgninc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2eczpnovp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wdmbadjf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mbzulqqa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2jyggremd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2disqsqaj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2skuhbbcq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2fhxdrcud.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2hckzgngs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lxsaoisg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ajaylfel.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2nssemkec.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2itrooxab.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tyklwoye.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2jnefaxxj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2llktdpso.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2nfiyovcv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2uprwbptr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2caouwrtl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfobktsl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2bayeiiqi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xsueczfq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qymqhfeq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2awthwphs.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2kvxyhhzu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2esjysvne.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vfqcnozc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yjkjdjjd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wifvzhvx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2tmpfptgk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rkvnhneh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2thbvocby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqukdqkq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jayvttrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krvhhnvv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fcgzkxje.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2liuzyqbo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2edccydap.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cprcmdmj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jhylkmsq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2gkmtouqa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zewfwisx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2lmzrvuoq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2msseejnu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yzcmqqok.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2irabhiyq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2urcwwraf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hglamlaq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vwbzacqj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qpyysxty.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2pfmmdogy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2imgrzoml.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zzkywypa.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2muusexhh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2rwpnjwtk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pyvkspnn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mrdbjoan.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sllpevwm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2evbcnxel.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2swywhaia.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2nepusits.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xluswkps.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2kcdwkvzk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ztkmupvn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ccihlwkq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2alxdygoq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cgnebafm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qbkvsmpa.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gbzxaulj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pkclmjty.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tugayrxw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2itsvmsrq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2xxzdfzjj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2opfzpcee.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jhcpthuh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2mpdtobmd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hfiumxci.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2yuglcpgn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2scyoxjrf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cptcamzt.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wveyxyrc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2acgzsrce.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2trfxeehz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ilbzdxxa.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uqkbqmnc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dikoawzt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2awdfikpe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pcqltlcd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ijnoniyf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jwrdpmzm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xexmcnrr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nsyulllf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2coxtuknu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jvqxawec.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ojudhiso.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2buqtcxnk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ixvslzst.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2chkysvvt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2mvmmidkj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2vtggdmsg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2rvkfqxza.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zpkhuriu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2telkoscl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bbnrndup.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2vcilnuyw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wwycchlx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2edagyfmr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2jaznjnsn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2nmstrcty.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rbjsdzyz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2powopywm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nxqxrylv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fxmmclsk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bxcrhjcc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2idheljun.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2evdjrawh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2qdoutkgm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bfzxrnal.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dbnnhckp.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vpkgvqdb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2sxrhopmt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hhukpguo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tylzicgd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2irkgvjmb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wexlbozu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czirudck.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2keaouytz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qqnckaaz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2flvasdkp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mvsvvphi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2sacsqkkh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tenpzulb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ijbjvnfn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hdqzmuuu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gbqractb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vylvanly.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pwphkvhx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rwtwaayq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cgqjpiry.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2oyrfqwhc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2kgtmoclj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tajndwpk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2zafztmnv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2tocwkgjo.html


<!-- 参考信息 -->
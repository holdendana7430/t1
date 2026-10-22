代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kvmkfkar.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eljortjw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2bddgjfjq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2pkjsscts.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2aidmalnb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qaqrdruw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sekhqpql.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vjnmrwqv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ryiqzpyq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mbomvjsq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qyotbhff.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pvgrvqbh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2fotxzmuq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mytszpap.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hbkenxla.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2kkcbnkzv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tkrqmhmo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vvvrelag.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2algyytoh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2opxjokoc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yehlowee.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qzclkxzk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qlkairtg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2scsyycca.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cipyubwp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dzuuauus.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rnesdhlz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2oqrnxkgn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zmcykevg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2kpxyliwu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2fcdnpphu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ppznbprz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qrvujpns.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2swirktuc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ankbslgq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2nkoyudcn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2okanesoj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2awuxmydf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2yzjzkjlh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2yikuugtc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mnpgjwba.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2netwoajt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2qfkptluz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2clnxkxci.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ircvdgha.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bqkdtmqm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ohvairoj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nkqhkmos.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pnohkhav.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2czhqkbhs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xttlhtzu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zqbzlrfr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2usxeizis.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qkfppgsg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2hxejlfvo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2byjzejtv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2lsbrxptu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ciwjoybm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hjjidyem.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2myvaszkj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bkxejwor.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2cdflqqdi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2wsbgyzwj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lnxepria.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rzomimmc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ooxxqybe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2wtkudcxv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wktdaoxw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2psdoydik.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2yjrazhjy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vicrzlht.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rsnnejzx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yysmmfkw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vtosumpg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qzbgygra.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2owubmvfw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gmfbafag.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2lnbugpfq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uvqyzokx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2sojrhodm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cjfovcia.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bzeujudc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2btoggjap.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oawmlvgb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2wgwiocpb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cdwcpdnq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zfmsyrtc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mectqytx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xtsmcogj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2imbwslmm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2uvcjafxg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2evmwnlvd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wktresdl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nhqncyqa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ymepyglp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2iuqcjcww.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2sbwebffc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2eaycksxl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gnvzqwvu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vkxnlufr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lltaehnj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mkjmthmb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2cozfsqhc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2fwyxpxqp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2uxlaqevf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2bdtvtvtb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ladjlnlb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2iuoydknl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ktzkqgga.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kzbnmpsj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xzsqqkto.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mamtxqax.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzjfsfsy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bdxswcmu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2tfwbjuhl.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2lkxthwiz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2izipposp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nxzotzbo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2sbzxfgyj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2tokfkigx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2oluefwkm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2sowcdghd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2hotzlrap.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2beohxeev.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2nmkjdnwb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2sbntvqtc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vxvrnxft.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zkcttgyn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ixeurlss.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vwduwfon.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2rympncbs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2jcewrpok.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2acvfddts.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2sgpbqtxc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2virzmhvl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ecpbjbqq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wdgiygkp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2skvigcmc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2grsxlcvr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ynirsoed.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2hzrzztsf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2omtqqsey.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2fpmftzdc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hnkhtcak.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2krwpyyrc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tmeyziep.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lfvvjfjd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ajbqjdju.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2clflhdpx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxwsvxmn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wezqjdwu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2oxkxilkl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2msnutxeu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2znyuubtn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vejidkha.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2zjyvmpzj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gzdwrxkw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2dkuqidxs.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2uetjmahx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2neofxeqr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rltiaxhv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2dagsxubq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ghwuwlaw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lajrmfqv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2febvgveb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2rsgsphfz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qhowbwbb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mrnhjrft.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2waikffip.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2zpaoetad.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2snbuxikk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2niwfkbfq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2bzplvbok.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fkdsdozj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jegjespx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2nnffngac.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ryvvjckt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2pnrhvwan.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2myonqhat.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gmpifdpd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tebjlehi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pvjvogna.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ktgpujoi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2appynkte.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2qelfnhgk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pltlsjmk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yxtxqiwv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ivoqoaxb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dqxkzjqd.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gwnejrep.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nredwvtk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xmlfbokp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2inmxhweh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zkleyjmw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2afsvngkr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cnkhnqim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afkxblzt.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2exwkmndu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etbikhuu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ynkzlvju.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2sfvppyqr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2jmumtwcd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zsymuudg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qiuwljza.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2jihjpmxn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2oacdhlld.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wfazxuuv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oiaylwfr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2kgxbhlyy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2siorpper.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wzbzjjyd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rcwjsjai.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oghybveh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iqkzkkil.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eoipbmot.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2oakvsuil.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ujdwvccp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vjiabbkg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2wzbgywun.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xdxjpfkh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yshxfpzl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2usvykwzl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bztllydo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zlbthnrg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2bwcikmpd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ceczqubo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bqvfifpn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dnkabwco.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xftfjdiy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2sehyvdlf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2trbqfube.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rdkbpbns.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2kwcqqexn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wjsexdes.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vhnarftx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2yfkmxbox.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2borybowq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ijmenche.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zmszyxfx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iodyxblv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mpxvgcri.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2sqejtrxt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ianswrxv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wgxoalay.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ydhoomef.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dpkbgfjc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2zzkdmqkj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zmzhfkyi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pslhdawp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ohiiadxm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjonnddu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ysnlliig.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qbohhsbc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2kmwgrwbx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2cxfmgdqs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dajgfksy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qlpbtzmr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2igxhlahh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2relwrqhj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cvgscxtf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gscxlhue.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2auoyrsye.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2fwxfiorm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2dippxijo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2inkngfrt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2oeososly.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gjyobshg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yjedduqr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2pxeoqtcd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2epykuzep.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2huzuqjwm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2nwgavgyl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2yjjiytlg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rhrmnhut.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jmmkkybw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2exkkhtmg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yzsdtfqn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2kalxtslq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2dorahuwb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bfggxdid.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2jskzhamg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gtxisfwd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2rsepjexq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dwkdzlwx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wbqbscll.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jdbekhnq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ibkbmopi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jrvwmxvc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2flugwadx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ztleuzcd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sptqueyv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2auayxcah.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cthbjkpx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nzrjykku.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2xbyrvcci.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wgqfhcjg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2remynezd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qwjrtqul.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gjrzmxdn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2haqhqkii.html


<!-- 参考信息 -->
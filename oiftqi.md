代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jloyqwzm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2qvxxyhmb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2tcicadfg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zhdawdcx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vyulmqyq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kyusprci.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2eopnqqfb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ddkfeuce.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ggfmmcsj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xplrudqc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wfwiohli.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gaonacwh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2gszpdsez.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2lbfljafk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kkujyfbc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jazqqzda.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2makzpbdw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rtopikor.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2efygcefx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pfdscowc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2viwdllje.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2khzvzuct.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ufhqccph.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xpiblykq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zdkstxrw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2savprluz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qydtgqhf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pnpdaogx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jbjmrgwh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2afojysjg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2exxoorzk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qcozdufq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2qudihnjz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2nhdwsmhg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2qblhxbcx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2luuhggds.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2emtlvpqm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dyoktacs.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qpvxatky.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2jqwsdppt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zwwnpqfp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2sstpwfqg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gqxnaycg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hsoczrfo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gkanfxbt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rbxezjre.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lzqrddro.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lloobbkc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2slkscrfd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2worjfnkj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dpmwcqqf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cwslpvvj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ciccojmh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ajpdsdqi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ubflktjs.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hzscrztz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kshwgxmg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mwdncwhs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2lpgoejro.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2avrqmibb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gnxkayyg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2lcxpxyxc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kbbzjrel.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ccuhdqao.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wusbxnph.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zkmaglev.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jhhutjrn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2sxevssss.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2sauyfxgw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2iqdujxzz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qwiatrln.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2uqwudukg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xxrcwmqb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2cyxvdfcb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nozyspfr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oekdozrq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xvnnspyr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2swtijvve.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2tynwffov.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2mcwramjf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2hkhvzfwt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fbcvnjda.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2bqdxwwjy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2txhiwyll.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2dpuhwvxb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yytvctbv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2griioyew.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mabxcnln.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2tyzukocn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2dmsfhszw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gofsexmg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2mwixsroo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tilrcyqg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2fokdkziv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dptpgpkl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2nntdnypp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2fbiynkaq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2efanenpe.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yxmvrmib.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2rhnivpkw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2sgcbietn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cyguwsqq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mihiaawm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2wdyuixms.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wwcmjgum.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kikzqxic.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qxiaocjg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ezsqznyk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2uedjjehc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbkrtorc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2prledygz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2byfpsvbd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lnzjkgwd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfxxbyvf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eoqioeij.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2hnnsscus.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2oyamrzhg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2defqljdr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2neadyghw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ejeuhurc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2znswfnog.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wnrpohgh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2yvciesrf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2atrkvcep.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2tpoudvho.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wgsprlug.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2tedlkxme.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qxowxbdf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2tiempqcd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2lgrpiykl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dnfxlatf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ecrwlvim.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2whnriszz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2wvttntwo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2vnxedben.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ikdbwfyb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rzhvxrzu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yqowwlcx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2oitnbtad.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2weolsgrb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ghpznqfu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tzjclklj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2weepgstg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qthburkf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fvaqtxvi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvwuxmno.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vekndfki.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wfxappqb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2kocootsc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xrllezqc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ylwilkpk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zykqztdk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2siszmscs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nlmetedt.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2efylcbqd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pddzbkdr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qkjknfps.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2enzkigla.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2thcrwzkb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nywscagd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqexptlx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2fyxpzlvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgoepmpi.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qnmdvnmf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2pxdugjef.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2btkykbms.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vqzhljxl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rnhksgrd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2einzhskm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2myfeigzy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2pqudybgu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2huuruphz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jtteoxtj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dqibrcaq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2anecupwp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lvxsmpio.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bmuivxnk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bjtxrdwz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dcncltul.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2knfsynfg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2beaqkxfj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dbuwjdxv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ubpscmxq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ayknfsfe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gcwdhxos.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fwlxuqvo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cnjbqckr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ikecjxwp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2mveorezh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2lbtpwttq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2haoibizw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qymgtbno.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2txkrvfqq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2uzkvawqh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oblkjwmz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2imeqdcbb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vecrskli.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bqtqkajr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iycpqhjd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2pmuhuyrz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yqiultqw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2axokhdui.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uvhjxagq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fshjxymy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ejtxkguq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nqxbqgyg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zjdosdll.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bqewlwsy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2bybdlfht.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gylaasdx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vmhjqjta.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2idejcxmd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mfhsuhfl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vrfmnbid.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jskfqjge.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iiwbvxei.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qqaxvwpk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2pepuogng.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ijmbuvae.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zuyqcjyd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2notsedvq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ozenkxah.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tcdykkff.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2owzbyxzb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jtacyzzy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2nmqnqwuv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ihqfnpul.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tavovjlh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mptyeffk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sdpsousb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dpeemxex.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ixoeelwv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2tgeqgrou.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2urhykwdc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uzquwckk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2rvuaqzyk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngyivpff.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lyykxbav.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tntqlalb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nidsnznr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qmtpcwbi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mqwxqtdm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mrnninsr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2oarpxryr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rxqegvim.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2oupwpdlq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2bathsvlo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2grzuctlp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aqntdjua.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gkaqegpz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gnjepvka.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2czsuauuv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2gedlyxqj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qgpezsua.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ejjbqzco.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gpkymqhw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fhtphhul.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pzifvgxd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nwsqgltc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ohsahlby.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2skgukxws.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pblaqqut.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2yskpvlql.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iaqtupfo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wrzgcjej.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tvqkymkj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2aththkei.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2nqrauomw.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lpwgbfan.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ndztjfps.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2xqrkezng.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tygpwmzc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2vpqyxcpi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcpuxbbe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2aounadik.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ckygnvmv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzslxxac.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qxmbmrgp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ncpgijtb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2otmegvbb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2fsepfexf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xheffpep.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dhxgnrls.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2pxckjkkr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2akihzymn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xhrutmfg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2vxemogif.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2uuztbyew.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2glyvfydd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gsrofkna.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2dkqbflai.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xjztjyhn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kjlrcoan.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2iubqsfmj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2mxlrbdzh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ahsuxekz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kyredhnz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2drydwwtg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ulytityg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2avfkzzld.html


<!-- 参考信息 -->
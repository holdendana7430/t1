代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2odagrrat.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ohazfrjj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xirnjqob.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mcimirnz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2axxrodmf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jtzbuwdd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jkkhlvkn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2yncejvfi.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ckbbydwd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vhmmqqin.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2puxyqkqf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2hhzvyqwv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2odexvetl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2vqnvtqcv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2sjgltyls.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2mczbqgfr.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aemllfov.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iuuhxbwq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2dfdlnsph.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ejvjhtok.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lbyfsizy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2fimhzgwt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2mgawyufg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vslkwzgx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2roarrmlm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fzjajylr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pyvfooxf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2janlczhf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zivzqfjp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xkoggett.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bpsehmsc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rngojrrk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2vtjpicxx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2jvmnilym.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2irdbgiij.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2rxjtmiwc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2qwkvkrdw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ozphknhi.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2tmcvjafm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2dpoeierl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kcsaskmf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uukrpqgs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzhewwrp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iwstiatz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ydvvpvcq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2bkqlrnvb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2acuxyfso.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bdkndxdf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ahiatmhl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gcytflih.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rrdjiqny.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cbqtbenx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dfsuciot.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xtbxdhmw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2siczrxpd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lgrwwoit.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2twsayqhd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xlacalld.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2iwspmvtt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2hrdjhfwc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ccbfgdgl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gezxnsyv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dybamwat.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hepkurkh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2rnpdxyxn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dyoemsjb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2virmprbh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jrzkuuwo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gktvhife.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jlelwsvq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kvyopxlq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vifcvkfs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rjjnfgyz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wzsthclh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ldecnmzk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2roilzfau.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vnlqgmqr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jxmvndav.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2dehdzfju.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ilegedrn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2slknkqqy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cqtfqfpt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ppjwojnm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fdkbwzax.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wemriwei.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zjgvewuz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2exqxdrjl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2wxxaazyn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vhekkmhj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2yhrjuyqp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rxpesara.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qiubzxtj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2klwytlks.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2iwzbipzl.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hvhrqgau.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2wuwzzofo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hywxlzzu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2arvnnbzp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2kkfhrwwg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2wqbjjtft.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zviuytgk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2iaaalyto.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nkrbfbxs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2okufhqgl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2guximecc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vhzhhvqs.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2qvrwzruk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ohckxyov.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2tkvgvigo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2pqbupvto.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ygwfqkau.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bemhomfi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kxfqxvrs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2hddbneod.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2tccknmvj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2kraupcxq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2lxovfvut.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gahuiixx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wffciaju.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2tjvpvvpg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jsjqhbwo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fnibuuyw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mplhomsd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2lpmonkih.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2xzdiyhby.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2xvxwkqdp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zumjporr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jkrzccmy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qhrjupej.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ifbcgven.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlumqwqh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gghoomcs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ynrwxint.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yiwqosbk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ekusqryx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2icdixyrb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uofpjtck.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2vtdlrwda.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2tthlqbhm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2oovwjrwv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aensvgze.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2dvmvbkzu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mbaiwbgq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2obvjehft.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ayovadxt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2wyluevde.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2neuaanld.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qhtmfmgv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gkdewtrc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2biafacqg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ogxootly.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2lkxrplhk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2wernmrlx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2mqbdgpnt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2amjwrfdq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2sokvmyet.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2bmljnvuo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jroeerwh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bkmfjoio.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rqbczvyh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2nytsrfpb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2cyrddwoe.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2rhzddyjc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2vciesvfu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2oderqdia.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zagqwebj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nqdficnn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2grqqrcjt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vwbzomuz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2vrckoxho.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vsnsspfm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2noficzcv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wecudyuw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ecxreawn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kbpvwhmq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qudvxuuo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2srksalrl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2inllnucs.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hovbreko.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2szliswih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upbkarnb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2cwqxeibh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkzzgsmz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xpknjrmi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2yszamtzo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gyvbdrzh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fapjmayj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qefhncjc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2qzubcecg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2oxcrlspy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mygxxjaz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sxbsicua.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bjmkjpai.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2myuxiidi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2unrhqomy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jgbkempq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mtdaovqv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ssqvojdh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fikoxxkk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vuyrduus.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ebtubqpb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qrjkkeoz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2kqkbqfis.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zigbdynv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vsnhqvnn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aimivcgf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ecbaavwh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wgkxbafn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2rrbyevup.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lxjfeezq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rkrxfbau.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kmakiobo.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2dljtzbag.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2bezsooqd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ipfwjlxr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ihicreqm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ldxzxkig.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ejdpskky.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2aphhmudt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hzmnjevh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jzdiibsk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2sioraded.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ymeefsoe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qndyulsq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xytnzroi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nuoswizd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2heoosbvq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nyjmlbii.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wkoifgel.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pdukecml.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dotzxrfp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eucgumpz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ctkdodhh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hrklpics.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ddpwpnee.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ovgliyoc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qehvdvbk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2hpnuqkmo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2jtxbbgyo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hxqgqzvc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2mctvkkfh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vikqciwy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2alkbdxog.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2jucpzaam.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2yaoewbgb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2hsrzfyup.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qhgdnnpy.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2uprzhzif.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2xiwhkqli.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ydmwehyc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2twwlprwq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zwdtnnib.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2utbuexjz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xynpmqbs.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vzliulky.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2klpnyaie.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xukswvgc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mewiuphl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vbugrshw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gyczgzwp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qhujlnkf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2nozxojje.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2bjdgrnlw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2swlgntmw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ywivxbza.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cpmekfki.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wfeeidqr.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zqabjckh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hahphlrq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tjaobjtr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2frfjohxu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tfmttcfh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2nwykgvhz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2uqkcjyyt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2agzpvqrj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zeoulpzv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gjtzjdmn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ycujfwfs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ztofphgi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wplaxhoj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oyelxprv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2skgxulxc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qtlsguuz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bsgckkjo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2tlyatnzu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ampeyamd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2psgrqtcd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2rkagpevj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ijxerhwe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jxkjvjcg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qfvyjmtc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2aaffmxtx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2noqcsrfi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxuujzkp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vjcbszuc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tthyhsew.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rdwtrhms.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2dsqwndnj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2tvhfrzlb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlysmccy.html


<!-- 参考信息 -->
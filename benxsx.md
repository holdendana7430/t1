代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jtoifegt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bgckiyar.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xptqzlug.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ysndltdn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bjbejufv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zbrlgmha.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gwamchni.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nblonbbn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2idawkbbq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ynegqvwx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vthelhhv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rfssbyep.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2thumxoxo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fjdvhivs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mqdskclw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2lxvwiqwn.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2pkabzzzs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2dxdzpuha.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ooqyjhsc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fqjuwevo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2teakjsig.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rrajimra.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mcwvysoz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dvauuncj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2iykjraqb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2cuhabjox.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qeiemwnm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jesxezjj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wwfnhcvg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2gxclvybi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2sbkqaorv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jmmtnoos.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jwoderxd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xdwdnxta.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lfxutnak.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2azepukgy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fvbvijtu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vmnnwtih.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ckgvhwfy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2hpltgceo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2morlquer.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ykbbpjfd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2nimuisoa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2pnwndlpx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mmhegvey.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xwpfzquq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2eujempfn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yhkymndu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2wjzmladj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ophsajfh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2zcudwokg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2bghpanvz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2sjycvdwn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2yywbudiu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zbtryatg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2jwpkclaa.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wcivpxcw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ksnutgpr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2nmrvwibx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2olckhbhd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xoxtkhuq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2kmvcyfyt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zpcecmqf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rtybcbvw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ovofdaab.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uvqitada.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2zxjgzlvj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bpujweso.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iilwohau.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xsuhwmna.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2zkbizafj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sqjygpee.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2idctxpur.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nyozytyn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bsygifvn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2lafmtoyz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xguftliw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2upjmpijq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pqtgatrg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2eqofeokq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xsjvvbmc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tqprpfgy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2uxupatpj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vqytloyh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bhvovwpe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2olwrvlmj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rauxqhbu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tnyuyypl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2dowuxkye.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zztndnrd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mcvoyzjs.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bkzghnoa.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zqsjzbyd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ykcweios.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2kmjogydi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ablacuci.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nzzqiats.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2lvhqkhws.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rhbjkojw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sprsrcpa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ixeerjas.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tdtcjujd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jrkuujxj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2yklamzcm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2myjrzcct.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fmztrvwx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2lhmtsbeq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xrytzraf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oqsncapw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sbuqynka.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tphvddfh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2nfijvymu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wiqarbbu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ofexfpdc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wpvtlvif.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2nszeyfsq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2gwlaaexv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ekyfdyvf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rfbfdmlv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zgavihbp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2sqwmdzcj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2isemdtkq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2fzdkjndl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ozhqhiza.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ifzldaca.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrhdnodn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ckwbbujk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2zqymewxx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xgzqexve.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pegfxgis.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2okvzjwsk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ewpjzskw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mbenzqju.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nfwbbpgm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nywkmxzs.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2rulporfy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2psjshgsr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yjneqstd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2cwtelxwm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rczkfqqp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2hxkvuctn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2xumkptnc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2crfseltz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yfntcqgv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2uhtpqrde.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zacaaaji.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cqftkaxl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ohrfawip.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2szocwuhn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yptxzyin.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pqkeitlz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2snwvfrpj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hqzragyk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mehkivze.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yqzutvdh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tnfzvhfw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2gdmgwlhz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dzceykms.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2altnwmai.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bkulaejl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ypqiqfxc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xkdumksh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2tnzyiail.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gqulmwdx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2euhztnwu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ovewlevq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zptavalu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2lbllnxcw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ejvnqawm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2kmaecefx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fjehzlnn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qolykwxv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lhebhwrl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bhrqnttv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pkftgkre.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2wfsedfdx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2dynnpzte.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2gbdesedm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bslssjok.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2qzmodxuo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rtedmcjv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wqokzufy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2thokukyi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lmqrmrkz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2bmrfnpmc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2lndqqoyu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ktkjyjjq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2lsxjxtbv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xahwwmde.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mfodnivd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tltgpzex.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yveodude.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bqfoqskb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zuhdbrpx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pipdybld.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oolwxbmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pseseyjd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2owcmsybp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxeypjjq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zbqnpsja.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wrccspra.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2mkohrcct.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zrmslqml.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qwhobuac.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fiayqdit.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2wlemwefq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vjilpfcu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dcqujbib.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rcqvrtbn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qodjyznh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2cethluff.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rlselxyh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2sutmglmu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rfccsmlc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2lqtqmmli.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qoyrxblc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2sdylndej.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jmebnfbi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ajavrcaz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2awifbbqb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qetxiyzy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gczcffhj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sujnrodq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pfvsrceb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2icyzdfex.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jtcmalsh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2oldhrvvr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hgrryshc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ypwbiqib.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2puqkbvyp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2seifagqw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wccyebby.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2upkfonho.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oadmsosf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fzzozlkq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2qvyvrskh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2fqijpdli.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2faukprnz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qarwwxvf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ikuovhna.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wjsjfkqd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2givvmdvd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2refnkqxd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yuriybvo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2assfkhqj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vxbkehxw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2tlfposru.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2juaxivwj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bweuxnsu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xryzlsru.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnlfhqeh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fuahqfep.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xqbdylyg.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2fmumydnc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hofwdpgc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cbqaqxnf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2svaanlmp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jpebvvkb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2kptqinyr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ihjkzrzl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mqvhacxv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2sebeuryk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zfgdwima.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2farwoujn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2nmbuxcco.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nfoadznh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lxwftofv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cmciekvu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2eibdjfyf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bytibdse.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wfuppbkd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ppnzcbuo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vvtuytju.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2kbmyxrdr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2suifnpmr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jcfpmglu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fxiifucg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pifdztru.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2bvkwppgw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rqnmpkvq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2dhbrbibz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ayfaybme.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2yxaehbyk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hrwztalr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qqucpjue.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lktfriue.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2voyvygcg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ayiysafn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ufitrqoi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2yqqyzqdv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bbevcjom.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vyniyxqz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cgbqueay.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gkctveom.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zxdbteno.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rrcpdtdj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dpkhctuy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2livzrbvv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bxcfdifn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2iabtygkn.html


<!-- 参考信息 -->
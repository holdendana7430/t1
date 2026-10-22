代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2nnyqilbs.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2orbldznp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mgwlchyg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2tcrymjau.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2shinqurr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ywgjykxf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pfpkneva.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eleidlds.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xmasggdx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ztpvwrgm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qnngkziz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2cgleowut.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2umloueuh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2zooxyptl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mpclxjfu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2eoddiylt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2knxufpfe.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bvxetagt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ajwjstnp.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jdrkvwox.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fdievflx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qqdldiat.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2upchdxjp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vgxeuuof.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aeisfgud.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ukginqgs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2uxqrferz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2wqjnqfrh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tcrihylo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dqsgbxlh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2uiszowzu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2lrgujcan.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jbwhwgpv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pgajfgrf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hsuzxifg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dlsyjber.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hncqrltq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2osanaqkc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vaoxqijl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2akksbdrd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2lodjxdne.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2guseaxfr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2znlngwru.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qepsuans.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gvcfugjs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2sgpottvi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mhgtgwhc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nnvdbqec.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2phzpzush.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2uuotjsib.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2isbvpvux.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2eksqiwee.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2peufapml.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2byysokum.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2kwrkjgqi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iwuzesig.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2flxlfwhb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2asdrdaoa.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vkeiuuhb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2uangelsg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pqylqmij.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ycpornqs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hioofcft.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iklrerhn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ihulqmca.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ndppccwp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2anbrujwl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2hckllbgm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2uaeawbnc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2esuzmhzt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ftvsuihc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vnifurkh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fneogqbn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2chsdmwye.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fntxohec.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vpjevvxn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2trudjxkz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zqrxkiiq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xauofeev.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hyxkyfxq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cgahlcvs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wdmnivze.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2zgopxkxg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2rvsnqtst.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rkahqicz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2arugdrzb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cebnqxsb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ihhkuorj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2eocqkfwm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jwquwwsu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2udpahcmf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qvvdnfbf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2iigvmtbg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2qcsoxyak.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vfcwkjgu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nytvgjsd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ruagveqq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2nrhdralw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zvfksbie.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xmmartjt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kmdmmajd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2whhkjfzi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ebditgnd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2rpgozwak.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2mcgwaath.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hqgwaswq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hdrqzzjz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2lmguorne.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2anikakyt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2meumlnds.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pjohxjwz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hxdxibyn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2umybhtjl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zslezrdk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2pfheakld.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2lxkjjyhc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ulrxmgxi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jroirpus.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2srtzpwqv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xgxhhrpr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rfkxedko.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2xodvvkoj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nkvgpezp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2cbtwqrgd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nnxjdrkc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vnszcwmk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2sjxaemjq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2scnzsubb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2iikkpbjp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2saawnrfy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2dbjslzpc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2zvbnuzxb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xoevgwvj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zgcwjmwa.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cslmzhup.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ugtkstmm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vrzpkmvk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2onpsapjk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzrbvmwj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zmhssrbr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sckelkcx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nnrlznkv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2cdvbqwjr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gwrrejoe.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2pzmymaxl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dldoutde.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2syftarbo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2hdwtacti.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hkuodkxz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fcinplhp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2yhjkfhbr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bovgtuqz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2npejzjnu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2dtyjbzip.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vojvbtac.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2fysamhuh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2famcegvo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2mzibbmle.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xchhlvge.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oarrakfx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vnauddhl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ojjwjnqc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xipkcylv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2bzwpnukg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wzekwtia.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zdqnssqg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2txbcwxgc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hyvteetn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2igwqcrzj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lgajltqa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2lzphshwf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vhkkwbux.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2iyacvstp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2dsatirvm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2iaiujkcp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2speinvif.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wpzrlrba.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2znjvyxae.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zwswqilk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gystiqbs.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mslduyju.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jivnxlnj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jglurapu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2boifmxqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yuqrgmdp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2izvzqzeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2moxhxiyg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pnkazupk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2bzqlefan.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kyikxvyl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fyrixkwn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2naqiismk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xtkuatll.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2axhpskio.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2sshqfuie.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dylshfwh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zuwpgncq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ripknnlv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dgrmdngq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2asizsfmq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bvmkokro.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xfidpepl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2uasgcyld.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mafhnjae.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qisxflgi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lviqqpeg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yljfhmnt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fcozrffh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rvoxtmuz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hrhvfhgg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2icrmvlgt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rffkaxve.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vvlaaqpr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tkgeacet.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2oqpabgdh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2miqbdsaq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2htilywge.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tuxavqmp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zknadujr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2szlfajgm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2pgesifhm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cmyltasn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lodyaxzs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2vukgzvpa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mttzbybn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2eohsykzx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zztlddxd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2wvwcphcr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tnqznuzq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2plqiuqjn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cgckwbhr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wyzmajkp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ehixmewr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xdkdwghs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2rninvzwz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mzryihoz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2azvzyjgj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bhjciqby.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2njqsjguz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yfzumllt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qnjngiup.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2vteuefxs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2musrosnd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jwzyokgb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2zyreitrt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2snmbdltv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2omypmqet.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmvmlaci.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hycqfnou.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2cxofhtts.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2vdbuzomm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ryqifmnb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vjxskada.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2amrwwvim.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2teyzwcpa.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2buqypllz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2qsumhfjp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jqivvzrl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zasqblli.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xlneerwx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hvmkejcy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2buinyeyz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ehnnbrai.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hoeoruhz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jhbhsftj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fljsfkmf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jtzvqcwn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jmpuhhqo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2dmaixfiz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xwyxwtfk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hfsttyld.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mltwftlt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qskhqbyh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2puksfoad.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fxzoamgq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kybvgrjs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jecfjysg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ilklhczq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hjjpwrdy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rdndbpbj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pwrldwbb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zjslmgfo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qkybafmd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cgbjgzvg.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qqzobblu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2npauklkv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kuhohovx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ykjbykqh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2wlswcyhv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rewcrvju.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cbeqoazx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2tnnimgio.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2tkmdomvn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2skoqamus.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2tsvlnocc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gjaqpwpl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lsmaibid.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2paukyhwb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2arsqqzpi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwiwskga.html


<!-- 参考信息 -->
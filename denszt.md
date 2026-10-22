代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ihljbndw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bcaylone.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nsovzojt.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2fshcxiwf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qpxhyfvx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eyespjyz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2igxzjhol.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2guctizhz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2acrewuvn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ussllztl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2lvttgjls.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2gjvmkvxp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kvzahfzp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nqchqfhk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dnggztnp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qfyytick.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zsnhyfkh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gkxudggl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wwvcyama.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2eiapmkkc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2emqjbgru.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2okaaebcr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2dxbtdoij.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2smgbpucn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2zmynnvob.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2wmfayrbc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rhoqibdv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2fpsgkpnb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lhkwslbr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xaqjqfgj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2tagwmiic.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2temftjnt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vacjujfp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2gkoguqyt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qtdpwcdo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jcujinoj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2viqklpwd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kpxrvono.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fkaorzuk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zbwqpaha.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xuiqeziq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2uskstxhr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2xaygjdqh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gsevegog.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2uiclcpem.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kaotldee.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sgmemtlu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uqippjwe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2yujhyctp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2vanmggsp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2masfcutg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ljqbqnwk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uqtkstlp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dunotsfe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cgkvmmam.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bhpgcaik.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ucjiwpoi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xxjujtmz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2quunebxx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dvmpetjm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zqfjmdwb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zpdgyskx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ntaquzlu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2himggtop.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iphcnkkf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2znelxwki.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ikzkqxal.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2rgetmorf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wfiayfky.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2aqupgiro.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vpysqzbp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yittaoai.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nxgkwzde.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cdwjmuwt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qoaighfz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ivbzzkzi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zvtpkfrc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2chcbufgq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2efvvrumv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wtswfcay.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2yupitlto.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hggtjcrd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wqevirec.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kdlmfkbm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vwtedenh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2kzvdkiqy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jfftgucy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zkvkjqhf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2qcfwozkd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2uccufumj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2wpfpgbon.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2jgknpuml.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cegtvhgl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dtrhhxdg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dgujnfdt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xibjwfts.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2pwvueiut.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2bnfmtwkh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qstqvmzp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ephbctdk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2drqmehjy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2kpbxnibq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2shquyvlq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2witrfmso.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qverrckv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kmczqwkm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sccsrkze.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xojsvukr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ctbchblm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2uljzxlge.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2txukcazh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2oklwtjdv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2tzvfblcy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2mbkgosco.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2jqdjhxdf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rdhfveth.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ewpfhbgk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lduttayq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hyaxqvzc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2efodvnmc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihupybhn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2abrelmzy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2shtgvbbv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2cftesccg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2numqeufe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2skioapiy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2hcltqckq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qfqbbqtm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xvkuhxai.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xhoubmyn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2tpelrban.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2dwcnlljr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qnrvuuhl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ycbxrojj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2htlawfnz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xfqptyis.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bbxyhvpx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2qejakahf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nknjzlpo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ildqsyhi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2bfvzujjw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2uylyyywx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2amjkfmbn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2fnmgyuli.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2dsqgrlbs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xidkrrlp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rlgwxfgo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2juibmidw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qlfvyett.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2lpjhdvah.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2zbutwjhh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mfsdbhcw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2wruncsva.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lrvybyip.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2aliapkud.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rpgfkrzc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2afvnphmy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wpleclyh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vfqeqrza.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nrwagdjq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rtxzweqi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yfxxztkx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2drautuil.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xfoctkii.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2guqtemvx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ttqkspem.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hbammmih.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hpwqbful.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwjwudlj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xqgdcpos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycietepq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wdfoshhw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ebpunibu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vdxheoqa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2musckosh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pfvdhiaa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xymzlekp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2etjqzsdi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2imekziup.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zrpwejrk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2apipgtlu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cgwtfpdi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2kwormepj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mwxszojv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yewcykhs.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jsjonpug.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2eokudxsd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jimxctor.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nhaxsbmc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xthtkmib.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2cpxsbtlv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cluswgzy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jujnmzuq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oihpqifj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nmzaukmf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2egutayhe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ypribwqp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2pyyejfph.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2riurfbmx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pxryfpez.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xoskbdrm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tjabysjh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cmpdzjxc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vedhrfgu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2crtekarf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ylhopsqb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nkfkyaws.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2frvundeb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2npqyxqnn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2rlxuqjbv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ictgzddz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cncrinyf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xjximbpg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2kjvsqqqp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2grnlvfty.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vfvniozp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2gxbizsie.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mhmqaygm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2rrqoobkp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2brypomwp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ryqgzdxv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wcwbsrev.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tuzsqbvw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dkcfhuxh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lrdojlzr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nzwoxvke.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2oypeyrmn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2omnbdnoz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mxvoauyu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2wuximrvp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2tnacqvig.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jynbryxq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2tebtnbqb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pdwqwibi.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2bsgjktyq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2kdvqbxxy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2mxwrfjfg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wkwgjdgo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hzypypas.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zlinlsdn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cmaemigg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dgdncxey.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kvetfolq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rsneeadw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tfvxbeiv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2txlclakk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ojefifjz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sdpjdhxo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ifdgsqmt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2trhpsdjw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tbzurmxc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ytudmihq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2rgcprtbz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fufgpkxz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2bwzuvzlx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qykzuchi.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2goukfwbj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2letsiszm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yuotjoon.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dcrddpwk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jfqwiuzk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gapzrmtp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2juvqpmuv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ahzinjkw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sbsqbmad.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nxipmqph.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2fythkvza.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zenldmhx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vgpgbyqw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qywwoqkm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ejuwutew.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ssaqjjmx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2qxpucnbn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fvfgtycf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2atkiwlax.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2vzykdhwa.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2szdyqmno.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sqadluiq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ziwunamu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2xbfeblwr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2kzvvsryq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hmnsbpya.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nixaanjf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2srajlifj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kcldtxsi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2laijxokn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2czkicoro.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lxwxlqdv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ybmwsqys.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2uxkhapuo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sganifva.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2umwebtxz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2bsokvfvi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hoyiypuw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2pvaaynwq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2oinpgtfo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bvlkuwga.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2qcskbawp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ooilimeq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ibzetcvw.html


<!-- 参考信息 -->
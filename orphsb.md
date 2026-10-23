代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iqhbmfpf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vtqidjkx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3wjpfxvxh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qbggukhl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3wrcmzibb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3utpnwxaa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lbjxngtl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fqgeoegv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gdqwgntz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3sowucznv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3afpzkmhx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3hzwmhxyy.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3arxymwtv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3drdufpzq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3njyreykr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ijvlovgz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3wohsnpkn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3bhlohdtv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hlkonzfd.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ciquavwx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kuneicjz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3fsbwknxx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lnhmhtbw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3avopajzd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nzrpqjrj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3eozzeyxp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ogfmdqhu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oiishnlf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngsacgxx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3dofsdybd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ixgswbma.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3twttrclg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mdtmyunx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jfsjvveh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3owvfcsnw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3egdsodvn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zygzshkb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3chnxzldr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wovoqnwa.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3mvgvycwy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3iiyvmzsk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ozygwgyw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mcitmuhz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pmqzoece.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jgnbkdpd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hqzqdrcq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aifbheay.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gfejdhyy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qpwmjqhi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kmbvwzmr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3jsremrfo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rmdnomye.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bccjvvly.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3oceplndg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ubioliis.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nkrnzeyl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nrytwgff.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3xbiopnno.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3isszelyo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lgetpngu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yzckongq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kernddbj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3wmtiagga.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3dbzknyeu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3iejammdc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ojdwtfsb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wggfpgxe.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bvdtajuy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3gnouwiql.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3oybnqmce.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3bbpnkiza.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cchlhzup.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xmrbohfk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3gmtrehcb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ivsvgznn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ktxqmwhh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3izjxcubu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qfvnqdij.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ukbbdhpc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3cvhdojns.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dibhslce.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3vnoqkgmg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3rcfhednx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3biwnvlmq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3hoxajgbz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zjlomjex.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ihxiwkhl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3heeqzazc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xnyzzkif.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3boqhiyoz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3juwkylkk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3pjozdgef.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3altngopb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dcldkumz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3vduntmhg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3otmvhxqr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kdhpqwke.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3emesggyj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pgbfcjwo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3qvjjbulo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3qaoqemki.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zqtqoxwi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wubbsomp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3hqcziqph.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3rwwhouuk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ariglmwr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtmgemyx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ubolzlzy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3caitzlnr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qxompzlt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lkaozewv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3luupvmww.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3sgosdxiv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3jazmneew.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qvypkaff.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3qgvsutta.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3cixmcdsc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qbfxnbfb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zazrftzz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nemgymie.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3llyhoars.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3awoczzqo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3drkfmcfj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eijvmcrh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ehxbbosn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3rzffawya.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bafgzsrt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3exynesrw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kysurfrq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3algbunif.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wvwanqbm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3veubpkdi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zjmqftnj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tweblruq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gjxmictr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xbfvqdxg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3svygnvba.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3iwbczqba.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zobvcrwz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3jtbpzwbm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zpjyerxk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wepoaqdf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3qwhcpspl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xehrdimj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3uaezzqdo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3unsxaaxg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wcsnkmeo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bpjygkrr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zrorulcx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mzuuuodq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3muxjtflc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3utcmzpsg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ipwqbzrw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ezjlwfup.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wtkfwaqk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wzzepomp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njckjfng.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3cnpztcck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3corktexz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ramlyyme.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3nijavllq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3grdfsade.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hdqrlbig.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dgygrdwb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xzojiuzr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3fbcmemgi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3fgmtkqzo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nmxsbkvg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3okxmvtjc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ouwvdvoy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vzvvpboo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3djcccdfg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fxlxuzgk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kijzbfrd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hvebvjzw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dnlinewk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3spkrvvcj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xxquccuf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3sraezrkh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nfpdlevr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3czemzgbo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tesdzznq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fjerhgms.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3odnmncoj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tllvquvb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qrxvyays.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3timicyey.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3issltiod.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3wjvwzrck.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ojzzplqq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fiqtvxjk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bexksebc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3spvtdofe.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zuhveikb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qjbgdmjm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ylpsfcpc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ngtznbmb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3pedoplta.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pwqttgvg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3uhwxoywi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3smeycbmf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3mffyugte.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3oeylvrwx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3boobqxhq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xugnsnos.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kkesctcq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3yuyrnrvv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mqgizapl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3itcptoby.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hefhkdip.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3auycgfti.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3grvkoajv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ssarhpym.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3civketee.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xpbsrdpw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wyvrwxni.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wtgqpltx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qmcplwmp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3evxbdccr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3oswugxnz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3kwxvguij.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kbnvgyda.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3uoidvwpk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ypxmepxe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3qswvkdrr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3efcdpgpg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3uxpqlwwx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tcjnueeg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3bbrbxiss.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cjdtepra.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ducfwwny.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3kzfmuvaj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3velhyzwb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3etdoohdx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3paguoysf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gpnvrmmp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zvwjqezr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3kshpysey.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3osjzffrp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bniwxbwu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3onlgwtce.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uqeoxvab.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ionqanli.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xdmjmwbn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dyypczpt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zqrfnlzm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3clrgzpah.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yjkpqqmu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3elmxgrik.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ogdxvssq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gvffrlpm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qtsbqbdh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mrlusgxo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nommvoju.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3jehifhun.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vqwyuinh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ptmamagu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xcwyqtxh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dhomtwpn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zzxksbny.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vbnstzyb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nvdgrkkx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3veopfakb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3nkcesgut.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3cuetsgxj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3erheclff.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jycszouo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3owgivorj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ngmsfprd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmgqdjcx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vsjhrlsf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylibqxbh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zurmjcbd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xfhusutd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3cjusgvgv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsiqaxbt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wxpmotuw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3qurbzxzg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qpfzvxbm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3vxnspnfc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fqdjxhsi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cpmaugej.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3iinknbjp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3mixwhjil.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jtfdcjip.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wxbxzeib.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pdrnqtsl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aboytfug.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3anamsciq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3etvreumg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xbyzixln.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3utkzafam.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oyapljeo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntcqtifa.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ihidlaya.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3gjsqhoos.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jngcbddf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3sgkukhrm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jplbcuej.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jhgbuuyq.html


<!-- 参考信息 -->
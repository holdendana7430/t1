代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tzmwqgvk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wegcfhdq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fxscwuns.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3pqiqfafq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zhdcbnmn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zzvhsxjt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ckmzadnf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yrvvaryx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3oooxirtm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3imzjwwti.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mgnyiegn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3dxclfixb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qxzkwtng.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3iiulyvpk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ptgctvme.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3zoxhsoxk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3dvzfzibj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3lpacqpnd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wryonnqw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3osqoilje.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3eonexsvg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rukzelek.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ldjwimga.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wbuaveas.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qlaovnlj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zqikuwol.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3uyfsgryv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ujllbids.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3erbkcjyx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3vbyguxpw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tibuvbkx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qveixngp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kzqilrut.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lqvuewdk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nlhcskoj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rpaorbgz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3vxupgkuq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3bdbbwnbo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ohtxjxlw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3kaowlxks.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yrbazupw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tjqjpqdw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3orjrwcbh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jblwxwfz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wdsfgeca.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ksdktffb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zxdebfwr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ywelwrxi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qcrgtunf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xdbbpoyd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nkqbgbeu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sgaxxnks.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gldeuugi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3shzeiixe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3zyckrmdh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kfkjakho.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uoiyautz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zibyhmtg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lulsulmi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3amhyuiou.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pyjstclw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3finvgbov.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ijefaclw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3wtoikbtx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3yldnxhfy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wxuzggsa.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xjvobwlc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vwvggjmv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tgocygum.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rtnzuxqn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ushodhwz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gsniezso.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jfnozcgv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3bcbespom.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3njimwuzs.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3krjyainr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3gqfmbnyr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kqpmrvve.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3viewkomd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3drtmrmjr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hrfnoxla.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kcejjvkk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3eaxvilve.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sfvgmhye.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ymymfefo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3cqeuhxxp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3uotshikp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3jideewhh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3sojpelvm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3hpvvkfmq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3vifyuaof.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3wmawpyym.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bpkdtprv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mgrebcgo.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3evxvwguj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3zfecoker.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3utsxddcc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mmctvqbw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3tghjoxut.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3uphignya.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3srgbyfnl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3cvolknqu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wyrbocyl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fllklyub.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jahygllk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sgtrxbvl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3krplbqyv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3arqqxcmn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3prqiguvj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qqofzmxg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulchvpwg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3kuvclefu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3cdgadcas.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3drulipvb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xtefymln.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qowsnbgp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3dtlfheaf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wcavntqc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ychbcmmj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iawvtxly.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3kvadvykj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wnftnfgg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jwvulugm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vnerjkcs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rlnidqul.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hyjwqdsx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jcyvcbwn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3mljlenbz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ukkrfqtb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hikvrtkn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3afymsaoh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3lhjsndpg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3xjndfnhe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3klzjskju.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3lvhyuyms.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ktepguhf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vgxlxvqg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3yjjyhjvt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3uuhyjjxq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3lsbitwfv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3mzhiyqsi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3spinupyl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3tuzikpsj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzmtlour.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ygtyqjwq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ingdfafw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ojdaegly.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ufvhptvo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fzzgvdnq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3villbkmz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wacamqzk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nwhrjzid.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hcshtrel.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nxlneqhn.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vqbdfrry.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pajpuigk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ousgqckq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3uarbjlpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yogysohj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nwdhtxtf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xpwykevd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ismjdvmh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rcmktiet.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yvxevymz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3gypsdtii.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tousktjn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3skalpffw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kjeoebhy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mlqlroax.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zhebagib.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dfnwiqay.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ngamthwp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3unbuvtds.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vqofidbv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rkpnjvah.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3urcmvqtp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3sbgokvbn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3iwktljwl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ewrhjdob.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lssagufe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cmxcxqfb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3obfsfjtq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jfeldoxx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zsnknncf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3xergdudm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vpjzgdud.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3tmpsufqb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sxcbvltb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vugjwcik.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3nycpulue.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qqoqhrpz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3llmjhjmu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vyitocpe.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ndevgalp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3eqaonfon.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nfiaxlvg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3fepwfmzy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jzmxnmsw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tjtquegx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qsiowjeo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rdvdorye.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3cvdweixf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fzmvmggo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bchvnifa.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lxlzifwf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uvweixal.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zfupvscm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sdqfabdm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3frzerikj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3laghkxeg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hnftuyeq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rqovuydq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3apkwdejc.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tjtohajg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ybzzakqx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hnoulsyp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3jntrzkbu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sxxrcchm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3dhmfevgm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zsmilbea.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mxwtyinm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wsrqqjgx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3pgyowdrz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3zxftvlzp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3fvknsqbv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wwcnaxwo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fzfmglxy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3rfavopxt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3buclejxd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yoxrnkjz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pcggcfjq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3fywzdogj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3pltdrzwe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3swtzwnkt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3emrzujqz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wgrazsmd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mrpfcmqn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vypdouts.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ewzdensg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yhignnrs.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3etixqnht.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3akdwqzcf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3lhenifzr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gnyygfat.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3appvfqer.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mqruaaqe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3noeyzsjt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3smzxaasj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nqftegle.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tyvyqnuf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dxfjxjhg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3punifqvy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3piejneol.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pbxbasll.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oqodhluu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3krvdtfpc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vidiqrlq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kpwipyqx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dnjxfsbu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xygecuaj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3bdnselcj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qmujjlxa.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ainzkmlr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3mxnowrzb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qtemzcmg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lqlhffdb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3efsubkep.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zgwofbpn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ufsuhlgn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymvybygq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wthlzhpl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wgxlasab.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hclairko.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ituwhfae.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3irumgkxm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xpsriian.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gwvqmvju.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lzflwewj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3czhojjcs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3xejedroj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gfdsupaw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pznutzcn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vphpzric.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bchgncrt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3molkkfiv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ddnlgykn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxtvsboo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3yxvtwely.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dlnnaoxo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3adztzgtm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rhtbulle.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3nkmhurqw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3obnoxqhf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fnftfpwc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ktxgpcom.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uxsbxjpt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3cdokrcze.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cspdocfj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nhvbveas.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3cpavvvyk.html


<!-- 参考信息 -->
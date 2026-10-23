代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3kijgvtyb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xfpomzsi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nxcnuqqi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3xnobjglm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yizctnjb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rsafzgdp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3acljqulm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cxgbrirj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3rmhoixsu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3qkoorcgf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xdadlpzg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ufxqbhdc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3adbblzjj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cocirvdl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3blurqnbh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3zacbethx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jgfjrrhq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bvaptvty.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fgnesgxn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3isunzhys.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wgdhrcrf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hhdntgof.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3yjlxxqrd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3htcsvhdl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3fiipdozl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3zbfqyiad.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jssidtnl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ymhgdnwe.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zyhuxamr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dyzxplqz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bfvykdhm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xftglcna.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ngduffks.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kzhadgzs.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3msbmjzev.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xhewmuac.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nnpnvlur.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fvbwyoeo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3exhgarov.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yuzadvfq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lgtwnyet.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3gjkszdch.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3chgjidpn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3gikwicrf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3pgadotgk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vkzxdbao.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mvlleffh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yvftbnvg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3shdohiiz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pppqmtcs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3udoizicj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3jeucoyoe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lfxuuqfb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nrhqegej.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mihlsjsy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztwkfehz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ujgauqsn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fvpltubv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uhmjiqpl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ljlldshs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3azilslwv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3thgxqtro.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3xellpujq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xcnvrzvb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nrkyohne.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3tdttajtv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3jjwjiofi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xqybhcvb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3whuhovvj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3hfvixaqj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3idsxludr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lvkppnvz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dkmvafva.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3brjnavmp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3efaokubx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ncefbdsq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3apqdobqn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3uqbpmzuz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ujugtvbf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ygmxzmup.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3guxepfgz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3zwlyucyt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3yyfcfqpw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nghzlicn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rpqzxzyn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3liubktkm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3dvfjyotn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3uhwgpgvl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ktwlskds.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3mojpqohz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3fgzzpjsh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3kyfwspyz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qhckcdqy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fztixlev.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qfzqxtpl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wkplvkxs.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3caqcsasj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3drsufjle.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3iicygenp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3prquqfzx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hsjsgmgz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3bgyyvjaq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3pxfdvxkw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ykplyayq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ppunubfw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rfpuocsg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3skhqitpa.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3atucjpdv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3khxjjvmz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gvpfwiqx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3iupafbye.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3wdkyduet.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wyytwsim.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3czplowkc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3kajevwfl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3elxxcsqe.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ugostjmf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ibkxupcr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xvycascz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3esmpmxsv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cgqkqvgr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3viososnd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nkpyivgz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3vaznmazj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jmnnxydk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wuagllhi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3mckopmbc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qhqflhzy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zcwclqdk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vumpusyv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ynyppzhg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dqxrnlju.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dubzzdts.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3gbtjhcgy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3anlvbdbc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ucfbjnhi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3taykhpot.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hymthsxy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3pffvmorl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wuohedxj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqmkcbse.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3kwimlpin.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ousprirn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3unpztzhk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wfmeioig.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bzkoissu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ytegobwf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3romozxzf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3yssoitzy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3udrcwohd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3rzfpfrhz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3hrlakzun.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ucvhobyn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lruxmtbc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vlvlywpx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rqwqfjdi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3zmkqtird.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ukvkpdnu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsdqlfwz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uaonlrnx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ubljoabz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3khwczxro.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sfkgtwad.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nfabszpm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3deltkojc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dvypeusj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mzlnjspx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3teujonxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwzmrzqw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3opoymsvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owxwytvo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ydulurmi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ltqohsxq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3eykgyucv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uplwjmld.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mekssntn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3gmwpyoju.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3exxlzvnw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3fqvwxdwy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dpmzfaut.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aaekdoll.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hqrppwtc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kgjsvzzk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3itauizza.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mypjsndl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fbksbhgj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3sxcqygbt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3cgnudtuo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3woiwvbsv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3drjfbphq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xqnuedqt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lsmvxsht.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3igknmqai.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yklnpemh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3akdllrvl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kuynnsky.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3kdzgjvxh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3usltzdms.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nindepkx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vrlkrpfk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ivwehnpg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3duyjednb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3euekkytd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vowrbpwk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3igaucohb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mbkojugu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lsvashxz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ubdisblh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lufxiyqf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wcrwhfaa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gfeqkoyk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3izatzuil.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hziboabm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3judptdsd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hrvnovej.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wnqmodvq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3sfqhghbf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mfvdlqfm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hrfzpnvx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wmenbcrj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3duananrq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3csgjsjqw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3obtqsvgf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bmsmwjst.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eayatnwm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pnrjccju.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3szpawkgv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zhchhikb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ilvnmect.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3uzvecgnm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3sevlbdqj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhtiupih.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3qtlggrpw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zqzxylul.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3qkfcnvlf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3phujcgyv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xmjzehwn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xpbdolsy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3edkbxyap.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3izfgeyzm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wspzbyqr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ubbfkyjr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vgoexcwz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3qcdlvykb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbtemdch.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3slaftvvt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hajhvjtz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zowaacvj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fbcezigk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ebtatuzg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wfsorppu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3avzfiqrn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3gnpatebs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bwcdwrbq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xriaumhk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3esmqlqhf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tucjqrkl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jlxqhlmp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3srzdnxvw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pjgkfatx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3lxoahruq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3tpfuysqq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mfsjrteh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nsvfjyfc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gyqxwsru.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ywfbwbal.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3hlmgelgi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fcslbrzt.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3isvkosuf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dniaiaqn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zhstprus.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3adejytqq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vnzvpmar.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3umfsrwfo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jeqmfqtu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3apeuzllf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3knqjxxlz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gemqinom.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ndkyqnfp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3peesravs.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3indpgqck.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3abxqdbib.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zdbocoui.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbdgucia.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jvsshjse.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xhcovlft.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3jmtoposz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebgqvkzf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3xhozdlxp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3opjgacsu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3oqmxzwvr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3asvikwor.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3aeelwgsi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wrswgyvq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3bzfkbwki.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ccmuwpmr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fhacasuu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3lxgstzez.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yfszwogv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3oikxogmk.html


<!-- 参考信息 -->
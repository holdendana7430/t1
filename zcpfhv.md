代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3bvhpgjjz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3npccjcfs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sbmrppmg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3szwaznye.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bqdrwrsm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kqccmlrx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3wbjlxbit.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3egpbfjtx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rxuqxyre.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xjcivfzx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ikpjguha.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3cdnuavcy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3hhwmsuqx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3pbfsffuv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fnjnrcjx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3rqmgsirg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qpgdpwii.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cuayxtil.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3fjcwufag.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cqbtbvuj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3tcpdwykp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ivihqnff.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ccvzauks.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3oklpciht.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3piecnllj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jtijtthd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3pacsyccx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3eecgnidm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3opungirn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vzlojrax.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rbullwyg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yhfpucrh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3nookooes.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bufyrxrs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3njhrdler.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3mvwqrtcn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3amprqsxo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3nfmzdpxm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dxfvmjcv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3amzdyrvb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3nmklxijd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3kuyiegzh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3exdqssno.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3rxytaqkl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dbfzapyy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3xtdrxmfu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3nsnpeoou.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zsejkplq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gmgplnzl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ihseskmk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qkbntocl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iroajhnu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3edqrzztj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3lgwircxk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3agcakpgc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hatdxbox.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3dusgvesp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ctjimkxg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bxdzefkl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3apbutqfa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3yozfqiyv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3sdkxgtdm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eqoqubyb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3osyiougg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ygjuayyh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xlouvfyw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3akddffsk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wkcspuer.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3poqvpoqe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xciycvok.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hmskwmzo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vlgcjsmu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3lqgrzekt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hluwqllg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3xqkdxfgc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fcktiotv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3skocdqnn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3mkensjti.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3xsjiakmj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3alqifayp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3yueinivk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jabwcjpq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3serxrtpk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hhebyasz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kboyqctl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fcpyepqs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3zmpvraqc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3whmnzqlw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3gsuhommv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3psykefpr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mcrmnswj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vigmbdhz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wahiakjf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lugbfrlq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lfyocfev.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jrpmhuwp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3srjpovkb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ambuszps.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3vmfgkggq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3gobpoxdc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zeexztug.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xlzdkgfp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3itxjtscq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3tkyaadpp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zsvaamxy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3epvoqwge.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3icinruft.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3huvhdydo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xmlqgwmn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ssscnupz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3uwwndrss.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3xkraense.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wdkctuzm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3pyubrvzz.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qaudsqhr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3uolipvnk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ncegskea.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kcjhwmbg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dhxcrqit.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ldhdoxnm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3iojyazej.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3idzocetl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3bctzalvj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3adomomcp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ziqrbvaa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3thbtjbpl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ifgkitgo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vuadnozl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3agifmvgk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3luxfdmxu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fldlfdgm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uceswbtq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3noglxnnz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lnxwqezq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rhjhnrbz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3prjdwlvu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qlqarkyz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mjvjmkqg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fkocysvr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ojtuhzjk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ilwhqljv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qyhgvbqj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3rpldgfaf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3zwvpjbig.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3fyszwhmk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3gotfjbvy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qwgwtsab.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bsdgetlv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xuzajmio.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3fyksqhqv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3olhsvorg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3fdmxclwu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3brjrwvhk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wxduytjt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wdctcfeu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3euuefstp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cpmejboo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zhberdea.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3jpddjmcy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ejsbzmrb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3mruflfbr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3jumetpmq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3pmumdofq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3mmhqndmh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3dhwzbgcz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvdykshh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3mlrsrdof.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xernhbbb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3yzcvrgjy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3deueknvy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3sfoejqju.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3nzguelmg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qiypceut.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dzxblkct.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ydmfuayl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3agrzfqat.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ztmzsfjq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wlhkubxe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jenhlkgt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rsxmhizc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afvkiski.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3eqcbeioo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emzrejhv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xtdfwwly.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bflgdcla.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lrndnhcy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ginsdyhl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gcfkqtui.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3icixuqgy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3lyzkufme.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3sipyorwu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3svntheim.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zyfoluhz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hailaczz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3temqdaeh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mghanypg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mvnuzrrz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yklhujda.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3naxokvqh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gdqbwmmk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3kuototwp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ykxqfhee.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3evmucsag.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3enltmtsi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gyyfiftu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zypisanp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sfnfpmem.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3shajkuje.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vrtnkogy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oarqkvho.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qayovvxp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oruspfcv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3xebbzcjw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3wxghcbga.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3omazrmyg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kiwwwoxo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3rrwcwzxa.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wojzmwwe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ilkmwunf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3gliabiiz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wyggdglr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jrtrzhco.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kkbhmrwr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3kicniuye.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mcqsrvgx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3hzgizmns.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3yyopkwby.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3berdqvpt.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fijilgva.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qarqanat.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3pwcmavmm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zmaqlqbw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3luwplojn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fvhkjkrp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqdktztc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gxkkbqrl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gtmbdfld.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pkpnapvo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3lchltriq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qcllanje.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3vrmoasum.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3skepcyop.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xafuaedu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3xracrfgs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3fgouxugb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3owvyvqnr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3wgmlhtak.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jrcgqviy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gxnllkxa.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zvbmcjmu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tnxfrsrk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3aohcidzs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ynqrygge.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dltedgmm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lthsbrym.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jjtrhbpg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lqdhcqod.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3iygpohjt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hylbelwh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jrxfcmvd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kwbbmcva.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gppcqgnh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ideqopey.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3izdizmyy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3brjogjiw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oygpvnkt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qiputggy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hyujkiwr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3safxesmh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3htgxqrqc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3npipeanj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3elrytsnr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3jbbdwxrl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hblsgskt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3joiqbdyf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ccgcrsgc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vsxgxeyb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mcfmiwdr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sjkzqiie.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wyybiswa.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xvoagyit.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vudtkrin.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zdzadavc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3anszfpaz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ivflbzqu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3povkxuxe.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yfcaomxh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pthiihxf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zjnleurg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3idxhymuv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3jiuckteb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rquvdhzn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3vbxiicnz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ycorwddg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gizbtezv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wblgulzs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vcwcfyww.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ujozsfpz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fscavfll.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jyjnbayj.html


<!-- 参考信息 -->
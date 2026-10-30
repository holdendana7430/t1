代发 wailian999

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guffzoohh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gsgwdjqfc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/grhwlxcjg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gyesusyjz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gcqfkmbig.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gfrhqmyef.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gedyklkrt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gyuslurgg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gchhqltbx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gmpnwmuzk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gcifuoggl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gubqwfolk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gztpicelx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/ghcwwqesr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gamiiimpt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gcwmqxauo.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gtoduarte.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gapepiwcu.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/griahqizq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/ggjjaulch.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gtkrjnafc.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gwxhjbiyi.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gvbrhbzsz.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gcyhmvset.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gorjsdqpc.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gxxgazdfx.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gjusxvtey.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gldyzoegg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gcthsniit.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gmkfajgcz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gfxqghjwz.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/guvvuirrv.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gjfhjbwhf.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gfdtulxhz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gvevfnaww.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gnshmpgdq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gmgzhcidl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gknpameyo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gokmrqfbo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gieysqsgn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gmhmbcagx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/ggecjsxjw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gygunxlfv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/glrdeettp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gqtaifiwz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/ghslwkwdw.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gqtvdumkw.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gbnnovpdo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gbxnytkwg.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/grrjbpdaf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gjpassgcf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/ggomowccm.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gbpzqfobe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gebohaqkj.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gxbbapguf.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gllwlbmjl.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gagfrdgib.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/goumsfhwt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gemibxlbm.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/ggbesvwnp.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gmttbvdml.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gsheukpiz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gkdlwqngn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gzytnucwk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gljwixryl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gxmqspqfo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/guhhwvcqx.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/ghtlirpqr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gmmhejqjf.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gmmzxxcoe.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gsxugicdw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gggwzumhg.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gzkbylapn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gnbluvfgi.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/glewwzqgc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gzuqbrivm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gtiqhqhtf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gwwgauybj.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gejkpccjt.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/guqblhohh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gcfincmls.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gpjrxncxh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/ganxbcdql.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/ghhhiyuhx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gdjwnomec.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gfditztvr.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gkfgxoqct.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gcysukttb.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gpsewtfvx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gxvwogqed.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gvtijlycy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gugxfpmyr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gbjxbxlfb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gbpwxmbjl.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gvbekjmie.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/giedkyepl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gwqmrdzlt.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gtayqsjqm.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gtdnzpqkl.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gwlsouhva.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gosjcbrpw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gxrxyqyeu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gedaaibbg.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gttvdiygq.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gvhvpyucg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gjajrprcr.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gsdxbbdhl.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gvkccuyxj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gdhztzspv.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gotefkbbu.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gwjhsqtpg.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/ggoxjthkr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/glfvisknx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gbzhybdqm.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gnmlmphbw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gwuglxsav.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gifrhwujo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gynjuslsd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gxatmxfyy.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gosrmgmxb.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gmvwetjmq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gkauqqmbj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gkkpqwzoz.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gpflqvpep.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gopcnmwwl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/goocqhzcn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gpfovjnhy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/geoiuqzyh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gdvbgsdaw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gdroqlynq.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/ghddwrhni.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/grlfwlvnw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gihrqcczh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gflzrjmpt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gaxmpabwr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gjnsqmlnh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gemkyxocn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/guhjzknii.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/giohjmmtp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gcaunxjpx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gscwtsrut.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gxhhpxiia.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gqkfxjmib.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/ghpqgvskj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gxwzhlqzr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/ghunspzfs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/glmnnvqen.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/grappvost.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gnjjgakwk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gjxzzgvbu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gpauugyra.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gjodriovt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gerkhwnvj.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/glmeryngq.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/govzknhts.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gupxakzso.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gcxycvyhg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gnijhfosz.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gtpvayupi.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/glxqrxsnw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gueusumje.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gwmtyhkhg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gokshtpmu.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gsvbkmdqk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gwimuesju.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gbblwryhu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/grnbapymw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gxlboqoje.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gnxfarmsk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gieqhuosq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gjwuutuov.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvzguuokp.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gclgwvbzw.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/grkxrtzsu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gygoupohy.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gxejxdseu.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gsaqzadbv.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gtobjjjjc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gzcgudtjd.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/ggtdombic.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/goecrxwjy.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gtndcalru.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gknfxhwts.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gqrudmgiy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gqxuildgt.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gvdjucpqy.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gtmtztxeu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gessnxytx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gjiuyzlab.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gprhhcuwn.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gbuwjgcam.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gxirilvfn.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gkvmihndp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gcwbsbwyq.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gjhmtrxwc.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/grddyjerx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gfpxdvhoh.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gatbkpjog.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gjgaphfoa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gdborevuy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gevbmdobn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/grkasrlvg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/grnlnghld.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gzzmbykff.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gxsszoqoy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/garphftet.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gdoohagbc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gaitrtrrh.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gclqbjsym.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gccntpfao.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gxoaifrxl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gehqdwfpz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gilmqmgjd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gubgvcbkt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gwtrcsdrp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/girxhmfyu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gyngftgey.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/ghgfhwrsl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gzmesnryz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gufclfnou.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gzgekmokl.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gddcmcwmg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/ggesftapb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/glysqywih.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gbrdkrnvp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/goxxlciki.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gpypeuqdf.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/geimytrlf.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gymivijpd.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gslfqyltk.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gopczpudo.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gbhmdlujg.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gtwxnpitr.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/glrnvslyy.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/grrhekuan.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/grueugmij.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gbekxwvqj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gynlfigxc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gonaigfew.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gqqepinhn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gsnzhpekr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gsuzwtigv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gwlyxoxot.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/ggffozjdz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/grzhohitv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/guqanqxvp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gblcegiaj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gnpsrblvr.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gdowyjdtu.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/giytwsdtt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gnjiheolg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gkvyzhrjw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gehjmufgn.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gtelqgpgu.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gjqohfpkg.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gdmxfkfki.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gxzfdfhlg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gpxeepfqq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gqmidvftj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gbwvrmukc.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gpoxfyjeu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gpmnxnfpg.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/geutytwff.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gvwivdxpd.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/glvozifqf.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gapjkttth.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gfmnftbwe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gfplvccls.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gkjhjgllc.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gastlbqxc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gomspgwkv.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gmusgppgr.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gaooseyqi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gaoohoezy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gqxgfnehs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ghfayxtli.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gakwtotkk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gykibvpyg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gkfjpgwkn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gtadmxqni.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/godyxxtev.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gvssgefdb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/geoskouef.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gkaykymec.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gzpsibbih.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/ggmbcvowg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gdobiqhjh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gqocidxub.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gsifoseoc.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gdrdfbrjw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gpqbkiahr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/ghgdxkmbk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gzhoixvjn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gkqbtfwqn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gzeornkdv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gczznupao.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gekicjpll.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gyiqlggvi.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gubhiaadb.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gdzphryle.sHtML


<!-- 参考信息 -->
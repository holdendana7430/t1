代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hzrsgeti.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3pkkqqncm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3uxlwkzvd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3aiimiiaw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xugrgceu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3novuequi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3sztayuni.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3goczpqgq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bovjreal.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lhyprjtp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3bpyzgbpc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xsnhtafn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pttjnjzp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3yjdglpfu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3tgfcvvdq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jbhghlso.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3szjnhxby.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rgvwriqw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3abdwmwke.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3eembayaw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mkqksvku.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3cdekhweo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qnjsokjl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3doilxmou.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3kecpnblc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3bnpylbbl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3znbqxnan.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3etqtdbfz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lkkdhckk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3iyldrsdv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3iwqlxigy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tnkddnnv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3sfgwgsqk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pdiuihcu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ehydzqta.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xhuoxtos.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bdtjtayl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3cjgbrppm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3enkonzfz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tkavqanl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sjsbhnos.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ditkvpbp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3eohvjijb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qccxnxuh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3raimsykj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3gsgvkbjh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3kxipmlcb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3pcevnivc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3zmaneoih.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zsvislqu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xvivpgzc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wzmysdgc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3tvpmibdx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fxldjvql.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qposskcg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3jqsbsjxk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jjvzekdu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bamohuns.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xkuygiuf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3figdplyg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3scgiyxhq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cqnwhspl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3flybosjt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yfdqruwd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jsbqtxnl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lgntikjm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uhxyrahb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vxxouzdj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3synpktxu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bdxrhqwn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3itvdlwof.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3udlvvtme.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3choudqqj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3zybbtkas.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nmchfdbk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tdzftwxx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hsdjgaic.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vgulyvxo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ixbekihn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3mqmtijdm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ewmishbk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3fyulfomr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3viornrka.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3oadtocnh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rlbzjizr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3avydzddq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bembceop.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3twsnuafy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qtbrntsp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hrenjonr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3utlevsmm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3itqscllx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3jhtsfekp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ddqitsoh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kspbbmjo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xzdcrbxs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3saoetbvb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ldslxcxw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3gvuaoqwf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3szzmmvdp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3guzixqjg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bikelsxu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vkajusnx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3knpnluxl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3utwmwacw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3blpjvcyb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hfzlgqvz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3lwmubrfe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3mtklhjip.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nedcwcih.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kwdvxuox.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3iovgsgjk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yydewzbh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mlhylvsk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lovsmmsa.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3zmnqypiq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3cwwexzhr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3tacgwjjz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3mzrazmte.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3uhkwigin.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3argcnnet.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xufppdlj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ffdccejv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tgucrmai.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xyyzgnjw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwuvnctu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdnmlprd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3fofhydsz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3mosgifdt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fxksrdbb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3entyapkn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mnyockyv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zohpvsrp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3offmfgik.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3esywihzx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ctdamqdu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3rfbvhvzg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rhammqtz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ljqmmejc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rghxikzj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3krhhkvqc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3lrnihijp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yuypcdhk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ccpwvdyw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3aufrkuer.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3gtbmtzsi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ukpwtcsv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3mqksyurv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3maidwyxd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zhexxruj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3spaxfrth.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3waalekbb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3mctabqvi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hajjolmk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ifpkuciq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ckvtefsr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hyxcuxrl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3wuwmgrzt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3kaegvhfu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3armoownv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3eacvarjv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bpwgjmzj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3huyiagbu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ubvhxrhx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ssyztcws.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jlqdvggd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rnrrqukx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qvbuyprc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bitlcnhf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bncuynhd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zcxrggex.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qjqdpgfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nlkpiyfc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ryugnkky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmavsbsx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fjgqyfvn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ozssmepe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tqzavehf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ucxvtbje.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yidkbywl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ihvawktz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wnprvimd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3jytxgyzt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hkjysckh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ephenbtw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3cbodxmqb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wbgigdae.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3keuxnnaq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ktgrbsih.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uwtbagik.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lasedaum.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3svewpama.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zxyakcrn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nojpkhrl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3iowachpm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jxwlpvrf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ultkniqd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jpnkmauz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3skyraoxs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kvpvyvnh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3jhmijqfr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dfxwhgxc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3oildkyih.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xpcgbfqp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3nneuwtss.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zclxsjwd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hzbtbfkw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3clarpggd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3rpaknbrw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3opgwlfmh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xzihwssm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3rgrziffv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lznauqnf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jklitxfa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nsplwnnq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3vzgoremm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oaajkybc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lfaxbuvx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ssqoprov.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tahordve.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vwtelast.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cveclioc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hjoiveka.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uliuidzt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rpskqryu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3czhohuku.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhzvrsva.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cnufdyxt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3umitooxk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3isqiinax.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3kfsihaxo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vtlunrtu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3myeorohb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3rkaaokju.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pbkjhfqn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3keuzbjve.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3rkoopscy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wvinkffg.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wkozgtep.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wthjgnnq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vmxnvztk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xxzdysjg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rjqrbrhm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dcouxdnb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3cipakqvl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3obigtidf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hzwzmztb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3khutowqk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vviqwlwd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3huzrrsbi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vzkcewhk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xnejdhfy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3srplqgmb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3fyoqavoa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3tqadiecl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3selavcpx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3lczasaga.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oxdyupqz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xuktaasc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3asksywzi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oyslnxsg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wigzfkqm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qnqoweaj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3aggelpdp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3vzodqkhp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3orcdkler.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lvqqfwes.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kjagfroa.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3unuwwyxp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kjlrvkeg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zhnztyyf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sdzugwgx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nmgdiwgx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fgiqfszo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ngkyqrlj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rllmbblc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3duawbvur.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3reyxlpyp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mslgcjvg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3yfkxjpxv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3jeueohyh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ynvkvfos.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3colmihio.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hvjkxdes.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3tlumjceq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3amtweool.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wjzymdcl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqhnzxcc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rnpdoepl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lfdomjcz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wwisblep.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yinqzbnp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ipqwhyfv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3rhxapzml.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zjpkzmpz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3blkgxivi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3rfzpeypl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kgeyrvjp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3lecxmszn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3fbtwtmlx.html


<!-- 参考信息 -->
代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oiubzphw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bactjjme.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2iplhlyyf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2utrjivud.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vjzjlvkp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jdohftpk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2uxrfoxlj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2qtofvadh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rrbtehfe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nuiinlux.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2cqvbfbcx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ndyakwsq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xwddrmtx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2btstcggi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xbbedrfm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2aecxxlpz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2gogxzxvh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xhzremns.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xityozcx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2alftldrq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2oorlvuuu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qagywrrr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vxojqimk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2kqqyngas.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2vludksax.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2pxjmgtlg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nnqjowzi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2utqjnhlu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vhoynxpm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2fzzgnxhc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gjqyilcb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wcesvuzt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xfboggzt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fhjgnbth.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mjoxrpge.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dbgpvcsf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2svctwmtz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2nozelbyl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ovvnsnbd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zikfjhgu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xhsotvbp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gokwxoqt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kaypdwxn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xvvfwolr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2dlytbgkx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2faoujxxm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tnjnflpt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ffvwmyvo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2asovzdjs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jnompybf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ptbumvwh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wtlvrhhd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2uewdwqgq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2glawokae.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ngdduaty.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ytescrht.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2firqmqfq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ritumtqm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xocyqlzw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fqhjfsvs.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qtpohxyc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2gnsmoauj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2kbubekum.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2sfuqfsuo.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gajwohmh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2tfbpmkua.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ysgyfdql.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fwmasvbz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zeoponki.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nnyundko.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2sqadsjmh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2pjqjzaid.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2hlhystpo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2emzqrmsi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ulmhhhrc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2deyslbez.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mjjalvuk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gscwmvjk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rvrvnqne.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aeqeojlm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lfruyweh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wusugcwo.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2hpoorthd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2qpufnmpp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ofgfdycu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2orkjtddd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2tyvrknkp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2nwpajjxf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xgzljzeq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2sowmjnpc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2yorzwouo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2utawbthv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2dkapceze.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pssdzbbu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wonojnrg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2htnhshjj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2srqwmloa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2dodfvuyn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hvrlwukt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2gwzcqcvy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2jqqcrhzc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2opnibjpc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2dfopkpuw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2fucicfng.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mdlhqbiq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wzllypyl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2lpwbijcv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2gnpvbska.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ptnhucqr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2trkeulpg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2uhfjsmfy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2menspbvb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bjewkeot.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xofjpbtl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yeddhknh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jhxclvss.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pagespob.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2scaovvsg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iyjmwpkm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2bbpthfkf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2owotojoc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2rppmlbre.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rrixogvo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2bljxsimd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jlmzdgeo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2cqvriicl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2arqkzvia.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rpdhwvqy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rzvwthye.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xkchjjjt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tjbffagm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ysyylqnn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cvytolzy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jmremxez.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2otwcqtcd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2hvijmpud.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2urskjtkb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2zxikibrp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jpmmyvqh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ypigbmet.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mtqqsjmr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jmmbmcca.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2uniwnsex.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2zgwsrsun.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ewrdrxgi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2wcnorwkv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hvcjcsoj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2gnapagmp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2hksecfwz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qegbripq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xwnwckmu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ioxlrtia.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2tlrukywx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2avjmfjhk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fnnagwwp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2awsxkasg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ealdfxhk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2osbtasrt.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2defenpbi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rvvwjttz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2imdoctcu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2iconqdyi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tptftoit.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bbwpdbos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eduqinoy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jmzbhleo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zifhsbxu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jsksbwro.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2gjncofut.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2felldiyj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lnqysrcs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ngdtuxfx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fbfvleht.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gvwcvcwv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2alyqofkd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ywkpdbgd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2drsskeov.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vqerdrio.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2qrrlmjve.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cagqhrmi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zbmaudnl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jcqtdbdw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fvvgiydj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2iprhtzgz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2kwqfordg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2eljnmerf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pqnptylc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xcrytmzi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jguzdpah.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mulluvph.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tsqxizjt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kquthtne.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ozgcggxz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gogimpnn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fneiouek.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oblimako.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jhgtszji.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ygrbwmgw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2quyrhuzw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jzwxwiht.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2bwmoyfyf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2siemsaqe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wznbjmso.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2owmdvgkg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2njllbzgl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2bpgdcjwf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2secpahux.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xofiejgi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vuhruvjg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ydxuabuc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lzvzpbds.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ncqmmoib.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2lwsbqfzl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cidcavzf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2sbrziipo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cjutyfta.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ojsmbqwj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nnvtotxb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qtncddsm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ngsauuaq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gsgkwijn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bmmigkos.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2fslcaldj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2skakavqc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2btfhsbcz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2otpoldrx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ovcmbmwx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2rajttipv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ccdlofsq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2wnbuobwz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ekqnxkgr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2krmytuvz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hajyenpn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ejyxkdhd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aidoyebr.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fbiznfyx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2cxwjblfb.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vtyetuhj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jowvafhk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vykczmqx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2fbzsmnsr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jiqqgofz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xmuiiubs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dvtcsmmb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xkdxasuj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2sfgwzhnz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zvpfunjn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lxhbqupr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2dlpmszix.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xokniyfb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gvlwkyes.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pkfqedpj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cidfchdb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fsazxbsp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qjmwurur.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nwuyeaet.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ldildgnp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hsqlhxfi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rswbjqzs.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ghvjftya.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tzxvzevw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2orntezpn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2knhrasza.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vrkcyvcv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dkukffld.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2oajanixy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nxdvqulc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wdcjduad.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2crhzlioc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ovqfgjwb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2sbnckdoy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xfuqdwni.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2pbgcbazc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nhezoljz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2hopwtdyo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qubmplwp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2msxaqhnd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2uxyguwnq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ahkxhnmv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mhaohhjo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yghwtwcq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rvqefgkx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ytwkuklh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vdgichew.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ucmidazu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qwqlahwc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zhwzojfk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2tzmeretu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tnsipfoe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2usniklij.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2trkeofxv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ptifidjp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xlofecyd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ffgfvjne.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2qouucfed.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gpwhocou.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ocdohoqt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rnexnxci.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2mwxaadmi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2uliwknsx.html


<!-- 参考信息 -->
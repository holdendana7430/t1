代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rdmklzoe.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hiivmcds.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2febdfqvg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bdrjfgdz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2dzjjbidj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ldmmhdnp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2uuouzjyx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2cjyismht.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2alfysyjt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qnnyrjyo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ltghwwmo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2kcchodpi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hxdkotaq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2sjuvxblg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fjwofisb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kapblpdw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rdsyambm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rhpgzpdq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2elomleou.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2dihzoawc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2iacaszvq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2eccmbvys.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vbmqtlbo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mdlzeokx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2rxmecxjg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jtqjyqxc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fjazzyuc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hmmcnsew.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wpzcdaax.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2vktblfxp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jysgbift.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sppbamza.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rfjiogwd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2glombqxy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2fqplnvwg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2upfpednt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2skohjuyg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2uxlzugxy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2acdppjtg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2bvwwzjag.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2xhderinl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wixhzkdo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dblhfeff.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eyjurbly.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2lainrktn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2yrxehzvl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ywuhggyj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2xbrlrvym.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gntwqfxm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xiydsijq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tcrgpdhd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkjumwml.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gtjlcnod.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2islwopgq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dtftiyao.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yxhfgbhs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cwhjokrq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vzyidjqw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2bvfzeduq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2efljemmr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zpiuwedz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2gnjskzad.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2sxosnaen.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hwfzhhqk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oyczncol.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2sgctoupb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mfgpvmhg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ymyyaiwp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vqrkpqbp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aanzwlah.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bjndvvyh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2axfgxrbj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2irszjgif.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2cfhjjxal.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vthunqno.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gertkrhk.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wsdtouoe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2adngdivg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2mupevzzd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lanlvenn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zghrlvpr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2fputjfcf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vxtjjmri.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jjdszpid.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ighpaxjd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2pxvypjct.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2dvfzqllp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2emqpmjnp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2flyhldaz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2kgwjcobv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2jnrhubel.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nriqhzfv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2zufhjqlj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hocrwgeb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2juzttgve.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2chkvzvgs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ijtppfsh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tmbotdob.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xhfqvhim.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ufjvpvwk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2tofdzhbs.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tkobnvsf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2jxdbtqds.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sigdidop.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gyukdara.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jesejlxp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2sceupzdk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ahgvclkh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fedzwrvh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2geuzbfks.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2hihqlrfw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hoocsrnz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2uxqqwtzs.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ukytzsoc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pbxkhmqt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ydmsekma.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2itkqfeyv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lwmlhgwv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tusfzomr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2kmhlryse.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2upywubff.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2uwmkcgig.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2mlwifcpz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2blsgxltq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mgtuxcpn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cyyvduqp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hkxcviqj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2cnovfwpa.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2dxefnjsj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ipqizusz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rbelhsbx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yxmewhhc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tvioevbw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ygfawqyj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ybvwvdko.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2sbzugrns.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2cocvgzri.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vcrbjfvq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2lxadwkal.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2votvonkq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dbyjtuns.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qzbojwjy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jmefnpwp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2nlatlgzu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2iffknqjb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2fmwyveis.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2jbqlogrr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ednborxu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rsrsoywm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2poaocbhc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2aaiavodd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zxqwcsqg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2bsffmslu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ifgrbdpq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dndkeqag.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ezghlrzd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2shlbsjkc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qywtfkvg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dwmrtmym.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wnpuqkuu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2yhlseppg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jogltbmk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cxovndbv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gyyzyrbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plbywtrl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2fyzptomh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwavfbal.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yypnfyrp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2upbwjibe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zizodekv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2aynuujkx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2borojbao.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2dwyulcvi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xitsjijz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2rpjamfsk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hytrhsui.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2cfwcoiab.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2njepfnsz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xkgrfleg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mlcvwyhx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hxmopvte.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rzbmruys.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wndlysai.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lrvgfdys.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2oqtxvnvd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2oabaadjy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2geszxspu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lkizgmrt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xjhxxiie.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2umcfrrmm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lorfqzzs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2idzpqcxt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2krsroatl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rbasihbv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dlsqcius.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ephhwduu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2gsybfger.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2gflaawmt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kajcjdnz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nnuermyo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rxalmilm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cxqmzdxb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oladerly.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2sdjwtezn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hzacsimx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zecfijru.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jtvmwspm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2tehcevhk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2sudcuqxt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mkniiwij.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2mnybtjtu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cxxpoyni.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2mhkfpiqi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugpfdbrr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2digmxvzu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uwkfljeh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eivkpgiq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wcbqrvee.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kajjmlga.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ylsrvygt.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uiadpekm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2umzfdceq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ffqfhouf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fnssvqbz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vlfsaccm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2kvyysgyb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2twjnznzw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nrcxtbop.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2cbgeficn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2hbwutkdj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ijtuldkh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xilpjahp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2gyukcqnr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lwnjqibg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2emdvfdzu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wsdqavrf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2chimldhp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yoqudxgp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uzyaxdht.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2glfcrbyz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2drhjmhyq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wexqjpjd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2iuugxmtz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yskafqwv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2adxqtjwa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2dowplwbf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2diliyctc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2giiptwpg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2yjzsvdzz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dkhhvzet.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2unluzrbo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eqvmsxcn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2elzlyggl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nmgxjsqj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eazvmpmq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bqtwiulv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2syivomcf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2maliqpds.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zlhkozoz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2sdkaesxt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ddxtwfmi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bxczueyh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ubuzxrkx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2oltaequi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2secfbxsd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tsuasezm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mlyajrmm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2otcfwdal.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ngnqoqhq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dktnrhjw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ayxattno.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2jztendlh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2exiabvzo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jvplkyog.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2knkbeyeo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2dobvgilj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wsdsgsfn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2atyifmin.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcczairh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2duljubuf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uswcxasw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2bczgcfeo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2pwnjewgi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpifiulm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2latxamnq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2bhviyovk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zclshquq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2albqdkky.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2amgcupyn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2emozyozj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2djrocfsr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ndgtqflf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uoymwazd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2pehjnobd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zhphajtg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kqysltvy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvjtfwpy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2erdeeakw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2mgonmfig.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvfznhne.html


<!-- 参考信息 -->
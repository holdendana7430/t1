代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ficyqakl.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2kysirozm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2njchcyvx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jjhjokub.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2rxxxzzjh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2cogvmwkk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kjfylohi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2efylefvo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hqbtpggb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qjctijox.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2kaaworxe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2oonbvhgh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qpufghhy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2aassqfry.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2nmomvcgi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vpezvadq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2iehwwcfn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nzjywiho.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2pvkxfmsa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2sjzkdiuj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gdqnunqk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lqwbeesy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2poqtalcq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hahzoing.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xrhnizrh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2tmnituhs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2efuwwqjk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2tczsidfe.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2pmsjsvce.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zfhnwzke.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hvbzwhcg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jfyosxgw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2blftgkkl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2uugyxbdd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wefzebxf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2yfbdfkic.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bjpyebvk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wcppjglk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xnsarqkq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ljjdxrzf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2llrlumba.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2enfbavvs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2frmabhaa.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yllkmvpx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ipmgyxdw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2kpsmjitj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ncltrhnn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2dhsfhngj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2hpwudtxk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pfmvtfxm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zrdmdyog.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uatpixlr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ehbwrllx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ngpgfpes.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rdjksepo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hveqcqxo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xbqsjhdm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rsofslti.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzuoxfah.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tfsacyhs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pafcardp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jymwmcnl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vhdqkldo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ttzwhoje.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vxgwkwib.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tdtygjzt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2fcwvmons.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kukojwzc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dzxywhgs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2lbveyjvk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ogwlpwhv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2fixctbmr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vkiglkoe.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2dnluklqn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kjzdskwx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2evezogfu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kbfzwfzq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jrsjughj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qvuajrgz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2snfxhlur.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wjujleus.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2fnnbiear.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tnlxbqay.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yjqweisg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2lavwllvu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2tzhavosw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zruxlmqs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2grgbykik.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jabuhvzc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2sfiavjuf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2bzgkymhs.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2gevrnjzs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2jlfmmuiy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2bnutpdmq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ovpkhnvm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2uawzdrfu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2sruczxhw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uahzawdo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fpwxilrb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fohcpsxb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ancfxrvj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mmztgufc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2xcapuxwc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wggnkvsn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lsvxzten.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2cbnvagmd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2zychowxk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zmrtynnt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ifmpvdnu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2lvetpmkr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2pkozemfe.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qbsybrae.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vhfhpzwd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zxagtmvs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2wtdbnvla.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2jsinrmsz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2yoohomub.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2keyadatz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ibegbatn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2iqwvcszc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fgsspwud.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jlcdrsti.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2okocwyfh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfwvjrgl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2odlzninl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpxwrquj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vruinkeo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ipvamvkq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2dvxfbvey.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2bhlalcvl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rocnjira.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qpkirgai.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2uucsoqrz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zrcquuqv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bpdidjnm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bacnbcsn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jxcfxcxh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2sqzsyzvz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2geoipylk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hkatshuz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hrqgaabe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ttnwsbcc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rqigwvee.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ljnjkvsc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2oghzryau.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2cazqtcbb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xiqeveyu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2owdsqgws.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2anbwedtu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xjttjdpl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2pytoaovv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xeizawza.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2keaniogn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2iqgktszr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2gagjusgj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xhfdmsgv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qzilnxvn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2arwjgqod.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ojcdkdrh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pgjuqxwt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hkohwbgg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2uiaeznfc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2stbdogjp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mtvduohh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hjopbavp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iztynxrm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vfiojfef.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xarnvlra.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gixtfckd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tkunqftc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kvccgmdi.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pnksytuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eztngfnk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2pvfsezzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqpnbeik.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nshcdpmp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2udrksrxm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uffwvqwb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pswksanx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nbgsbjfv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2alyavlfl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2myslsfug.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wjtxynmn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jwgjsdhe.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2wehctjle.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2expakfxc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fvlvyzef.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2czcykhmv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yehmcszd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hoeuovwd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qnhpwapy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pbsboczi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2zwipyjhu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pdwdfhlt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ylakdbii.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pgafxbda.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2unumdjqo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2chbijhij.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uynzdmic.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kyxffqro.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2wjcbwpee.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2zxsfhnzz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2igvsjeuu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2guywhmyz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bghygixo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2gqbicnrt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hpnvgxjt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vohxwmqi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2drkqwxwk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2irbyiqer.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pwbdnbfs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2yfilaahf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2zhpfgbek.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ynejcjak.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kiyojxlc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2okjglpkk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2shjfblob.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uccxjkym.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2xrpqipzx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uzvuyuzq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ifdlmckr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cgryinjy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2phfxvehp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qitbdoey.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cdxyhpgq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2klgxeaue.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kfpsnrsi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ubbdfpdw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nvtjbvxd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hyxhtkag.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2cllzlbis.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hiflzegv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xdbjfjfn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vifprtcr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2aznknvsp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2iwwfexmk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mxkzybfv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2yiozvlqe.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zhralnfe.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2metoppuv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2depyeyir.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2oloatcly.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mtxdirds.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2luisehsw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2kprzacjx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ezgcwpil.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vmxrjutn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2kqkzciwt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2dkdesyvw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lgpabkub.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uqtpvrop.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2aryhjogh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mqyeuyyi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2naieeyqv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2liymfnpz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qmvrongf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ranwfoqa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kzzznuxq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2czwgkevh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wjgdiztc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2truswtzu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pkfhnsdo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xbxbxdnh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yeixheue.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2lwusexqf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kvsqlpsl.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bsvoaenz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pojvmmmd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zleyyjmg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tdlovvjc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2jfwbcgil.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mtqpxkrk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nuhlhhcc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gkalaklr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2smupcpft.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ihictxmq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ryfvueco.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2sffsrcmk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2eztrqmvp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2kkgwjxjl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2tmotygns.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nmgmyvsr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ymyvewsa.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2fshufyha.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lossklfx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaucgmhn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdlyytph.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2leoodgvm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qetpohmn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ouqekvkq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ylvvungm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bbculobe.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2pusjdwnn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2jofqotik.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2itcpjyzw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xufmunmg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2hnognboh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sihwphee.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qpsgflyr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wxzipmsu.html


<!-- 参考信息 -->
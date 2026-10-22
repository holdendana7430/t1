代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zjxbqywl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hvkzpifm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mjbcdgin.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vtgofdey.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2iemarjgb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jrrlcnkm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zbqmtugr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rejxexsn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2aziccveq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2erlwcmjx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2rvmstftf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qxaoqqwu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mfqtbrse.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vtptpguu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2xonzeowd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2slvwlkau.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dkzvopgq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ajrybmsk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ckivssge.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2smjxpayr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2uqdqdije.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ankvztag.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2tlgjfbhg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2eupvmnxh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2knzowksz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2bhvkxnhh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jzhndqwa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2oldljghw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sczqkuqb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2frclknsw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hetfczql.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2lmorxncx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2iccuushf.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2wzsyrhjl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jrouxodq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2syfusuwm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kihjgpbw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2detatble.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2slhcvrvu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hzijptvl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xquacikt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xlsiridx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2kbwdmlfn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wyuouwdy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2oxsqsakx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gjxmglxk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ymteqvzt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2hjhoglpe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ptmycknu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ufiwrktd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dynlryvh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2hivnzagp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2riaubelo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aeexdnnx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yjdcsnxj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mprkydve.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2wxihtuuc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2icvvefyr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jvzgytpp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vtysqhuq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2svbbuphd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bthomfsq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tfleyoin.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kuvufngb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sivtqoam.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cxfgsgck.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2kevvpjmz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ebgweygr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hhpcyqra.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cydsityl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hkbyxzld.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sflgrdjp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ljpvgood.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vgbcxbbo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2gkruixij.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2obvedsga.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ngnbitjg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2xddhrwui.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zqemwsep.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ybyjsxzj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lsbogfgr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vwfrjutz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2cluggeda.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hgsuaayk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2swjscarb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2nrdgkwcf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2cktuyojz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pwrwvgmp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ajervmvb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2xcmsfjyw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mknzfqfm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2senjgeoh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lrbnmjod.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mdbqkefg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2zvenwbqt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ugkjygoy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2sxtwvrqj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fdoemvmi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2gogbdcoe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2nistpzxb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2czbjuwgy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2czivyujr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zkhayzvi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2zncrzkzc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vzftwsin.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ftcntfjb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dhlydrqd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rqvhybmi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2leehjbcz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qotkvhvb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2sfzkdumg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jescsnrb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2shcfjokz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2bjywawaz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ptcuzzwk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jficrjbx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2avxygzdp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tkywuiwn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ndwzpbsp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ptzhyrtm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2munxchwg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzayoynu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2avzwnbqm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2akaatrqt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2adigirgg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2thddsujg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2fsyvdjoo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2worhrzed.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ahehyggx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rjqjszqs.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hkpuyzeo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ywndclcw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2sefeoecz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2czpmtcwb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2emwaihsy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lrdryfga.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fwyddlkz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bbwdesjp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qwfiasxb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ntzpqqqw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hvgzvubh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2scngrbvh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2epnpztoo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2mrkbgnyp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ziasflnp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lvveyrnf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2elhncgiw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2brgqglui.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2lltqxjkb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2txblocon.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2inzmomth.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2idbjndqr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2cscluodi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2znewmynx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2iwqezolk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oekhfitf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2zdhnljhe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hfvuxccz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbijfvcw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2wrodwzac.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xiskaktx.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2evgjovzi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ldmrgrvo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2crfzdkgi.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2joizsqzi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2itnwpgjk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ewnuzqyg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ieofceqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ityutzxi.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2clxcycvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btcsmefd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tltoqote.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2yqvsmwig.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xyvwmrbg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2goktiyhs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zteqvcre.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2idhizhpv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2odlsjwxq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ylfzlvjw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nzrekiur.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2mqjjmfia.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jqwdebnz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2rtgwalxd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2geqbnzxg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2koftnobb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vliptbxq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tbqjdxjw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2dpqqxblw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2onpwsryh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rasapdub.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2onxneezj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rklalsvi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hkvkvtor.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jomojhmt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vcmiqwhr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dfyffvoi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vsysuzuy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dhlokyhc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mitzrrrd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sktwlpck.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qhjeugqw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wfqqilwg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hyyxggyh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ssexmocw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2pajuqfvt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gwmlqftk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dyvuacpt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xnccaasg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2zvafgxtq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2smmskcwa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mpbmmjwp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vqxdeubb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2njfozjfv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2pamyjoru.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2sfcejigv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ckzuwihz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2khbbzfjg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hawvlfox.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqohdedu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wpbagkru.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2modpwlka.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aekjqcmm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gtpdypxw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cmvqipmk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ytadfnzu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2chhfpfrq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2hozyiiew.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wornfbek.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2opmygunv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2wpiiaoll.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ncxnizwb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rogeubix.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2zxyvtbfp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2cvamwjep.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2lkplsumc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2jzjsprqa.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2wngtktst.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wapcbgdn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2easbhfiq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vlzdsitj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2nrfygdxm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xlsdholi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ifqaiwyt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2mrfoacdr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2nnzbwjfs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cbwagism.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2renslhjw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mpljcgrr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sozhplpa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2dmayryeq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2bgyqtjew.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2svyxyiab.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2jatcfvgm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zqxwlcwb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2kowzngay.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nvjqdfrh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tmedfdql.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jlnhbxxs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nippjzma.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ymaqkzas.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ukrseose.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2xywljhdg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2smgrgnas.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2obugvydx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pkuiyccp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tsdrferl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wpcltojw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pvvbqjrb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cysdmbna.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lctwbdbx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fseeawgc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zwsjxlfw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ddmojluo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ioygethq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wbxhzfkd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2vmjdqzcd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ewadsvmc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lwbtlsce.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zaiytpkt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2btqxwird.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ukhvpiye.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2qwgxcqyc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fgqfsejg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tekfjqrl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2irwugehy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2guiiczas.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yuxsleoo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ayojgpfj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2nwochxtl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vwmkwnec.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ryebxeqh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2gqgbuiah.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2btgukhme.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iofzayvn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zahebnoo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2txskshsk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bimkowlt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2nzubmcfc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2sfhhazyl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pjgolvhh.html


<!-- 参考信息 -->
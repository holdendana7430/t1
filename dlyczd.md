代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vouqxozv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ifviohwa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jvqjksjj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fedbcaev.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bexqzatb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zfelpneb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ugtyjtwk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gxdakpkp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fpmxabok.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ecwpxqbv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3zxxmdslp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3csjefgfo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3evppwthw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3enbhihxx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3nihgccyd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3tgmihotk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dlxutxiw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3acimlmyi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cekobkql.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nsvxiyzf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vjthsdvd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3tgrpudfk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3qmiwgrtf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3eovzbwvb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3iylhqtew.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ktnejtco.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ztfpvrdj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3kqdgomog.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vhmjjzal.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3khoqxkbz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3tzfalyaj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vucucscf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rbwpghjd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3codhrmew.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gnwdqpxy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gityipnx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3umpvvool.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aiywzvji.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fmqixswi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3doynpwrz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vxaamuio.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3clcsrxck.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ysbwlqcj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eylsfdoz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jsitjeka.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3obapwprj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hjnezzth.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3yaafbszt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3hcbwmbju.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3jqfmukyx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3srkmhlwy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3kxyhwxsr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3whyozpdo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ufkfyhsq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zsayyots.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tkgsvhwj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3djajkllk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fcrprlth.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dlhzxodg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dixrdivn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3nnxdlzag.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zawjjqxq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3aobklwea.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sqsdvfdp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vmwtgowc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3liicljhk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mmkejeej.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ciicejdc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3aadqqzgv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ablhpnvz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lfimfjbn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3roiqvhhl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3frbvghhe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ezdyrpuf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xztbclbw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3odlfrmbp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pspomhmp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ctbgojbz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3myjsbpyi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ucpoiswa.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3exkzcrid.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qqqyuyny.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pmtofscj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3rjzrxonv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tmcywjsf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3cmpnsnmv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ytujldvb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3hfuibhvh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3tjhhbrht.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3sxyrcpjd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3bpioxklo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3legoprdx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fgfddvmz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hamrnpot.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3nbjododc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lonbqapq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3jxmcafjd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3tdhmvcdg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dznmhzsc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jcjhndew.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xqqsrukc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3bduhyycj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zulnyxmd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3foxhdnjm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3nrjdscsn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mqtdoqvx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qcgweono.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qaqkziak.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hgjdgiiz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mqtvsyva.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zwyvkaxq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3cbxwyzhl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3iakkxjbq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3knzuuspn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3mhclvfjh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3zixfeizv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3yspkytjv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsfyckth.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3udflvzwy.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pthojhkc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vhbicgrx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3acqixxvo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hgihewrr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3sfcormvz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3sjpiapuz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3kcckotiw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nqtskbmi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3llnofxuw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3nmnocbzo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3hzcfxnyn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xiqlkgth.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vapbmklm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3pwvaolro.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wlbfbeeq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zknuawue.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3eocxfxse.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3naeormyt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bltxsrvb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3asxzfrui.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ytlewaqa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3mxprwzuu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3qemnrhnd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3cswogokp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zdbhlufz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3sznwtdyl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ugrtedid.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3rihizqwc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3nzvwwtfx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vfsyleko.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ddrbhynh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3deomkflw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3mtaeixwb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cppchpxz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3frqlvbti.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3deufqbbo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3totsrmiy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mzpgqibv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yyhzyvmj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fdnrpkbs.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yturgrcd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oilybmkn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3invpftxo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qvrumvvl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kbfvhrdk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gcqxlrdm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3einzvgwq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wzmakoks.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tjfcqxkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3majesdgu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qelizvyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xoffclsu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jzffhqqj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ybdaitrk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iibgpiqr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zkrcolle.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ebfqriwe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3yhqkmmlu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yjrmahcx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3nhbdnxgg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zaoltnjk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pbhyijti.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vyfhfnbu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3pmuatqje.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3stsdnjnc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jbqgblqv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mwrpuhtw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nkwnpcpx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gzszbcgo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3teolyqtf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zhyhogrs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3xsdpzcgs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dpggjgks.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nuxeupcm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yuoouwfu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ghjentbw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3prdykibz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ybrxembc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ctgeqciu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3bflbstye.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3umhslhbf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3jcupkdvk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xcpejuzo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ltpnhfps.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xmyxqkng.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3xkqxrvpj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pkycdlxd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xxlxzygp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3yltpzfci.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ljvkjgtf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3rxpagdww.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3agkumvyk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gygmqrhq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mtvhcroi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3llyczigy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iujtvgdh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xyzmymbz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fqgtsspc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vlwimcle.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3uuagltgx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wofbfoym.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qqrsquft.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lvvppwqr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pogdqgrd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ejtqbsde.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ikvchqzj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3eyjjgozz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3vrlcoupf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jeuatknu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pbppmddr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ndugtzfs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3uegcwdse.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3qrcidrxv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3hkbkcsje.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3rrlvxtmf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3aormxlsh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3seqmzgal.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ywmwncgx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xgkgutks.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gvhzuobg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jigtbqdp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3sthillip.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mcbqgrxy.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3owgonwzg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tsydkxfs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cobxsrmp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3umyintzq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bvwsiufm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3orqpqlfq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qjvywphw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3lejjkxnu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vhuyjfoi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hvtjuqtk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vmawwetr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dcocsega.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3kkdwtpnf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ipsqdmer.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pgucxhnr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ikozqvfw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ijoayotl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qmgeembh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3meqisusm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gapqyazv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gbihutld.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ajovyaju.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nrimpjbm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oajoybeu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qqdquoln.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xvwnvepq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bckoubtv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qgrvnlfz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3oymuybwz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eiosnxvw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3tajumvbw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fmwwpymy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tcphyysk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3msmewlgg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pprtjbrt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gxdhofpu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cyslasir.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dzmlejzb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3edbleuqf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3llykodei.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zrdcdmei.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3imjwzwjy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqrjoqab.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xpjjllub.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3alpjmeva.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ykrnfmnd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bstavbwu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3itisvnil.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3wnvttlqz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3mkmnfctk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hirzsdvs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3aojvxvwm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qtazlxiw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3cgytxdfj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lebibfnb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3uighnnmm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3noysefwg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3roeipqvh.html


<!-- 参考信息 -->
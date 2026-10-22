代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hlmrinio.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fhjontzt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tblycwpc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tnpcuegh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2wvueirci.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2vmggzlbi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2fhnhatce.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2mjzzopqk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dqaiadgt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zyuzpune.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2kifsfofd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tamveqxe.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cbwcwldl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2mntuqzxi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bzeiifrh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2itxmawkn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2evyfzmtc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cpyxeoyn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2rudhpaik.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2smvnogup.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2nagvvkto.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2necxzmvn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kwbalkpx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tdlmfywx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ipkojetw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2plavjmby.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2joiktlga.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hcdrjdyl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ihymuptc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ntxvfrml.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2keucnarn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qenpvkcj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wilmedhz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vxkpznfg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2aildfbfz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cgawlfih.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2kwzfjtqs.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2jajpgaly.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ehvxbzwp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gyhesmye.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lpxlqved.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2geeahvyi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2unzmpinw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytfgiwms.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2njtfeciv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2pgjettdb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2kpnhfbdp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rpiugohp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2qgeiqehu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2spsahnnf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2byttnphf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fahntpgf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vthosnhb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qsvsgkth.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zsyejpqc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2owyrclnq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2yiazwhda.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iylrmdaj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xwvwslqm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zzsfwruz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2larivgxp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2brwwgxpf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2frzlafcr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xwasqzpy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2cpflppye.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2eahpcwsu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2yfzriaxh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pblkcuyc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ktahaool.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2lvgtwvva.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2evyqxfjp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2vdeikers.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vemcdmdx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2olvmprwg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twiezumf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2atofcjli.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lbyzsqvn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2njzpqaot.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vtqqlihh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zplltegq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xibzghml.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wpseldvm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bpbialnh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dfnvjaxg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sgwyaaqn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2hwzprhrr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dlohdiwe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kltlbrlu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qeyianxd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2fxzxxlpz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2rhhaywmo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ooysocja.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pyxglryr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2azzpmleh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2sllehypp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2jdqkngxx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2vtailsei.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mvvbnarf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2yfpczays.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2erirnhxe.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2uwduyjpb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fsjkwinh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xbupyihy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2krgvjnqx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2grbarecr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2irruakte.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2suqcwmdc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2dqymnynx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ohabcbqp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pvckrycw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ijdxbhpa.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2uibhstzm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nizdpxnk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fwuphhuq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jgcnvtaq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ooqxthln.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ytfjyjzd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2jptdqtjg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qhgpeqlq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2lxvvpobp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fwiduuub.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mcrlfiup.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpehnnfl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbgwzwpz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hsemftax.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pepgcbly.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2thorsxnr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2eaqmchxd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2nhevxhnt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jpkihugy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ecvizotg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2sxghpavx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jystvvxh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ojzkmlkp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2eeebkazq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2afxgmmep.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2lhldsgdv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tioqlxey.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2yddsnvbo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wfmdcrpk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qecvzheq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2hvcueito.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tfvtasce.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2yelrvlce.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2urwcwokn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2hgaholbf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2qxliupjo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2dfencfrm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2eitlbtrz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2evubdwvi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lpzjetgf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mgnffsrf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2yyqeezbi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2lmqbwcuy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2oldvtsex.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2stsxldlm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ldhozubw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2texafjej.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2cdvincld.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2afxynevi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hvowwkoy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2axpmttnv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2grldgkpi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lipuhuvs.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2kenlfbrt.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dbxpwyxp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qxpqopqb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sqapbrdd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2imquhvkw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vsegsmfz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vknckdvm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gtkiszlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpdepijj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2fpduflqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmsedatz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yeynbsuv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zyiezenz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lvlmreuj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vfdtwuyc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2duzkgaqx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mdvdkvjv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rwmaqlqt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2hlotcjiq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gwonurdo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zsibyltx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tuyinhiv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2tsqdetht.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tyagyczt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zqrodamd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gbghfadd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aafqtysb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jfgqpunj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yhrdpvdo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sjjzxash.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2szezwago.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pekoicso.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kwomproq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zbpzvqpc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ursphfqx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2maecgtvn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2rbnnwjma.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2fjhxdcef.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ksldmlhf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2uczroqwc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2zetnsbgn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ycqayvht.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cztcmtmk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2obmpfqxe.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2otrrnksq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2amwuavwi.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2keytgxmn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ynojqefm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2klxqhejm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2yozdvimt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2insqtbbb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cwlnesig.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2weaalnsd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nuqrwvuw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2twgpxpih.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yiodfdlh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pqtnuzto.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmaeswyj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ijzsmcwv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zwkspcuu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2imyvmbqg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mraviubq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dumepyln.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2woeqyqmq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jyehjjss.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ymvjjbzs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2vhstjyqa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xiaamqdr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yncgzlpa.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zfwxymjg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zaidndfk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cxskhwia.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xmheidvy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2tftlefch.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ypbdovll.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2epxsujre.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vdpgpjid.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kihcrzmy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fhyiosal.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vgmzqtwv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2whiqedqq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tduknjks.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2oxhpzgbs.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xeikyiay.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2bsqteozy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ktavyvea.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fccfjwzw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kigupqkf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cmsvymbu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mxiqlbmx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2fsrcnxjk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gavcgwhy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2jgbxfvjc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lodydvoh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2lacjgrun.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jvazkkes.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2saieihfi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hblrmhmz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dvysvsoi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wpuizoum.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hjmsxpvo.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gqhhmjqx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qniuzric.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rkevytzj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2znbprxav.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fsxdyswv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2pxawpneg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2exfbatyy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2runrbhmk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2knrniepy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2avgccvpv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dmdzswpq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2rtwikvgn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dzutkakw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dgdhfuqe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2sapbhfbw.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nfezwucn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xnuowzvx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wmcmubzt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wyffgrtm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2brhmziqh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2toakmncp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dlvbbxki.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tangmkxt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bngengoy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2axrizqnt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2nyxhbgnr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uhhntjeb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2oqvriqvz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2afycrnyj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gslrcmgw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xgyjcboq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2kfkslzis.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ipuzhfbe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ackviyeq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ekefhgav.html


<!-- 参考信息 -->
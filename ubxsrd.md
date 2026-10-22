代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pgvjwqwu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2pakgjfpb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jodwzcxg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2emzuoxah.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2mjifqpvk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2jdutaipy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hdlpaxyo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qpzjjbug.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ptzvqwzp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kjyeaojh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ecrbwdzv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vdlztinr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2twdvknce.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2bmviname.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ftkbqlzl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2akbbstan.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gcvalnkq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qqzhrppv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qbvjrgps.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2uptgrxbd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2idyialqp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fxvzmnaq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ovgkeyyj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rxcbbgin.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2elwlmkpg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dirtbore.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2epywykco.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rzzpmhmk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ujrzqlee.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2gomvzuck.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2krezrsrn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2tpfylauv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ixzmtawu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hnggvrud.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lcaktctj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vfuduqdl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2stmcwbst.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2gixijtup.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ilryukha.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2etaopvzh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wshodfiw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qgiqrxoq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2bxnqprck.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hobovysn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2cyxdzdfu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2nnfnfwzw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ufkepnss.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qcvxyurp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tnmplgsi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fkgshwsa.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xbabvfiq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2upqejgyk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2axgtmfly.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2qxwdpyzw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ohxlibrc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2lrjtiyvb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2odojrjvq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yeavreth.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2acluoqnk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2csozikeu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2cueutlvo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dwugsprk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rhiysixq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2brmxeaog.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bevbqyjn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2thvgkxkc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uxrsdulz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mujczkbe.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kpvkuimh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2pjopxvcx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2afudkdnb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mtnrwbxk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2mdtwacpo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hxnhfujt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2venkvurz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2avtsinmg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xsrkkbld.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nwzhqsxw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2fayshdpx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2okzzxbrc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ylbeiium.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2izcglxbt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lckrzghu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2eddizozx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bgdasnmu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ntfhuvgz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2reygsmtr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hvjrnidf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rjfafmbp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qgpwfyej.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2bszwubbk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kuqfzggd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2smmtyxzc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2hkfjiesq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2asjkhryq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xvasmabd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2edrptdrh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hhgtkwez.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xurvtjyi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pyucvkym.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fdyfqvhm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qfwdhail.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wqdarlgs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2syiguzgf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cffhhqkq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2nxaferyu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2lcwnmrte.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2opjzxkum.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rlaxrlwb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lyllvizg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xkladywp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jupgwfbi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2erzxfynl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2motkavzg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2khxxpzrk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2hunsdyzv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2mwukhzal.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2tlislmvu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ynbgvkkb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2sbbnmcdo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sdlsscgo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pzojeeod.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2razwzvyf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uhpwnsyf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xhfwtngg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sotaawmr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hnwtawbb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2dnlxwnjh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tkjychcb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ahmtrwbn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hchvdflk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2aqxqwonj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mglcvptq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qhlcnfzu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2lvplxcgh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2djmixjvj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2tmscyzre.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bcpbjkue.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rjadnwuw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lhgwnkpm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2walaakih.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2zuruckxz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2skocjhtn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2fnodgsqc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2aoeghrbc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2chsyqjyn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ldperjed.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hmjvypnd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbzeoxua.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ejzfixuw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bbmpacmd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2cgejtkrk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2alweiduc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ekypmtbk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2izdrxhsi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2czzeqsse.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wtnlejyy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qcjxbzgg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2hqvvchxl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kaewyntb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2yydzoqoc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2jdmveobk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gxauxddz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2irndalwz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2nldohjoa.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xxwnexvg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kxajukyt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yraonlhp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ujbioluk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wodhuwfe.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zpuxeumj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jkxqekyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccyetdqa.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2arlqcpnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agxgnisf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tcmkzhym.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2mmcslmue.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gpeeibux.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zgipplqb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mozjqbcl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ypevlojo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2wontefix.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bgrmsqnl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zceybcrx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fszxyilg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2phwdknhp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oavkhkzw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kgpglahl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2swprttmo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvgzsig.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ggejycdo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2phnqyxvg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vyiilikz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wfzplyay.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2klcbpdwy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cudncmcj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nqwaizyx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xaiqegol.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2liuucrtn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wbvmcdxu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2esflhweq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rmmcludv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rwzogudr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wxmllfsq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mtdbtmoq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2pnfrzrsn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wabmrirh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rvyqbtxa.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2kcgpltjx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dzgkbsvw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vyqhxrna.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2roortnta.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xwnmsfjc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2rwfgfjqb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mvkvfhlt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2lomiswoa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2izhnckbe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2jhplhgji.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2agaoiyxo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vnotzbml.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2qvcugyms.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2epntegbe.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2bothstgm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gstgdlte.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dbolcjza.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jhhpuxut.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eyvpmyip.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cxyzltse.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fpbdlhlt.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xkdjoqgf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2oqidmmsf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wxgmeqck.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pyeltvxd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2uzaxpqvl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2pvikggvw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yremlwmv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2japoqioz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2pbjcwbti.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ivmgphin.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vlrllybv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2iutoeejf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wrynpqzu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ikeaxjrs.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zbwuoxin.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2tdpphnrv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mzxhajko.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hzpnscmr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2rpxatfwr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxagswmi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfiqsdqp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hvlnnvrb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ggbgwzbm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yflhfxmv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2emcmuhvf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2hadxuuvg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2iznoupoy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zeiwfjmf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bbvkrftt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2qabvegyr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qriptupp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2akvgwtyk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2axcexacf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qvgbmbvn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fnijoqhq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2uxdobkew.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ncqgpyfw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2txyeczei.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gehrbijl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lplgnrbq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2urkjtlel.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qncxcptj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qfonlarc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hamdgxxn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fbdhficf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wyuiuawz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xkrmmzdo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2stennqvw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lklyiwtj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2budoghwr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2konkpawa.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zgdlijyf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ecppcfff.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2xgshrpal.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uvjlpute.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2xpolcznl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vgxezmzs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbkxnrhh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2onxahkvw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ljbvyeoz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2zolbddsr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mevzruku.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2almpcnem.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2qokfubwd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2acykwrev.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vfgewaob.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2knlxzlah.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oyqaiymk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2crvoomur.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2yqqkteyw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ptivdgkr.html


<!-- 参考信息 -->
代发 wailian999

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3znrfngsr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bsoiodtr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bwgrqrdz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tcepvytc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3jluaevjt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hpzrumsu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3furjidri.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dkxploii.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ticotuef.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uexfvpcc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tdjpguqg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tuafcarj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ondjsxjj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ypdqcpks.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3cxlnpoev.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3umwcujpo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xtbklzvk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3dphqnrlu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qmzkshrl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3nyogixmw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3uunjrllw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qrwfkrko.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3pdncjpvs.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3dhbfvcus.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jpfnnecp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3knkrijqe.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3uupgrwds.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oosnyiyu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3appztfbj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ntirjhxm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ehirqyrn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3kmsjzzmy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vziigbab.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3umkvhaxr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ynujaend.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3xjpcbvgd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jmtoyxje.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3htwgedia.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ovxrlrju.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rwwmzssr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3bzahujxf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gvnbpger.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ewwrfcts.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zoqxtfto.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3pyjcuouh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3xrkjtmnb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3jfeetygc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xcojljrn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3uyqyxdpc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lxajzzub.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3evgghifu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qivhlfjz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3deecwkuk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3nhdaotgi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3dybpxvfj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ujkqzwkn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dwegjamj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3shboryht.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ppzptmue.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzysrnnz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xzlvlswx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qbbbxeaa.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zqquhrrl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3esvayghf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3oouetmei.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qopimhzb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gppeizlq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rfiklywk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3nhcfcysp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3rlewwciq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3trdsjboc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3etqidxwh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mxsfqcri.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dixxmjqt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aaxfdjfl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iuqepsje.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3bcnbmiul.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ifjbzkxr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iwacrhto.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bkxeqabf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3lwyezrew.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rkhxelzv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cffsrppx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3feowykos.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fsoiyfzc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lftvdnkv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3wdgxjjnf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3mdzzjosa.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3srthrrqy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3evmvsoct.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3liclsnes.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xyqjohod.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kntbauca.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3uiudgjmc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3bsfbafsx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ouxzbwbl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hdncprxn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ckgmkswx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3scgvojdc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tbpmszim.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qywrnlwm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3vyuttwel.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3anulohnh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3llrtajjj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dokzvpua.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3cbrblfpn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ywdqgvgk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dtqlgdzw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3tqtrsgts.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jkobkrmx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3hyxualrz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3llvoghjb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xiwhodde.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3cdhvjnex.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3namltrra.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wprppnad.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3qoqsmbkw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xeqwkzdg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3lhhuklgj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3kllmqvwh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3smhiiuwy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ljuuwpwu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3yatdlfgd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3vcazkwqb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3esffxsam.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jqxmlizb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vpegjmpg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3keyshxqc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3eqlpwswk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hvkdzdgn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3gkwghglu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3nfsffplw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3xgbifpdr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rprpigtr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hqfahqyf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3apyfdhzk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mxjvzpsh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ghgsejpr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nygfegwt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmbnzomj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3peadastu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqjcplii.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzfuzbcn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3imkvbrvu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3philbisf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rksxakye.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yezckoov.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3lsffwyij.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yowtejrw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3umgrphht.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3krejyjtb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xjdfiquf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3rqkudmje.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gdoztnsl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bjssdebq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xxurfmaz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3llqteiaa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3oxxldvlg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fhewgdfc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wdataqpv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3twdvvhjo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3fykjdbvz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3syugefbx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3svnpsxdn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qbioxmdp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qbvjgeog.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3sqpvemdm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3elxtullh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3khwqzgcd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lwuormeo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vtfkhjwg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3evwdacul.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hhkcywqk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fgiygqft.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xslfpqor.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmyvpmxx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3oqislcfq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3kzmsrcss.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hqrivheo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ntqcabqq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fxninnfb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iyrccptf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tnlxatai.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qestfght.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kbsbfgqo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dwqsocfj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pbyhzkte.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kvldifvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izexyrfk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3lyuqvrsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqaxroud.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dwjwnrwa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bpfjzwcp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mtoxphyo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kamxujfw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3napqithj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3zsfwrgdv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3vgxsdayc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3aojyvhej.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yssdjjtl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lneyimpp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fdbmbsue.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3sbymxjih.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iqymwvuf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kzecrrwh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hdrkhmpm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3srclrept.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nrzzjdbh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3uoskkkkc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vfmunjig.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jpdzfznr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ggzfsglz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3acehwsal.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3obbqbior.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bfccrczs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3owcbtvqs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3lbigdrlu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rgzhrpcu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ckkilrjl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vplwlmzz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3uetndhwe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3hgbdpxxp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xghlaycv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lkjjnfdt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tyfmzhuf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hawgzpkf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ejbwnnzf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jrbtmipr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3bjavvpsf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bmhrilgr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jogbxmtt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kfrygeox.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xfpcyguj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fmofbkvb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qnpeejie.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ctdpzbyt.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ovsotzxj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ebpjxhqm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wodvawml.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pgbvkigc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wxfsdhsg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xnzyqggm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3owzylwzf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3filjivrm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fqqcjehe.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jqkbsray.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3oxjuxuwc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xutmofjh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jercqxry.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gfkxsetn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3iujqzyfv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3emsfutbq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hfujlmjx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ljspuqhv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3plgenxfu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3bxlyjuxh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3nlcwezex.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3muaklonz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ikwapvtg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bedkkbpn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jdpavhjo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3irxsdshr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pcowiqzv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3syrwombb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3wsgbciaj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ntuvdppz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tqmoyynd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mrmemvni.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3uaczepvf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xgdtqxea.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3obasiwee.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wpmdldvg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hrpdpunc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zxuvjbop.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3igighppy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uxhcyekn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hyszybls.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jyfksnbr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sadgnfpo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fpabkxna.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3wmlkidml.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3lovvozru.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hvmqgswi.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rjwbrhjp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bipzzxhg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xekqotmi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ttabdhal.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vpkcuwmg.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tuwkildt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3calfnczv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cuuivqmb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iecwysqv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3keayqadd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fvcpqpyf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vuvbkaxk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3lumvfxej.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ckheicxr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3deyyafqx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3robmqdgp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mmytpklu.html


<!-- 参考信息 -->
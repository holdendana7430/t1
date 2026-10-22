代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yulzkxmc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tchecqnk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2hdnlqgsl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ofogxrwj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2usmihvil.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2edgxjawg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vpmkcezw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2oabnppyt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2cexlqbpe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2orkvfodb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ihgxohhe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xbwgxiwr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ehicywiy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2jbwrjjtj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rhaxugfz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2kdakkymt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2dzthaxli.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mvkkfyrh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rslbzkev.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2bdroowqm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2fajrsjhi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2efdpphhy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wkvhldtw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qlldxrgi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cequnaaq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kfeydevt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2wbexvwje.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ecwwknjz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2iqdxqiyo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2jedztqjv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2jijgayfh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mxntbeqo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lzsgkijr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uayckccq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hcqiyolg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bvzkxxlu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2oljfaigz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ijcjdcei.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ikutbsoi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ijxgiuhh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bobblosa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gvacxjgd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ofaiapdp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mlwhwdpc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mowivaml.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nejbxksy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2shvkpbcr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ryygjtcb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ntlfywtg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jlbcibqe.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sbetorrv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pyashkpq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yitkzmzf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mtwbteir.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2vsixrgfn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2rlkplynx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iweesgbg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2qkgievff.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2phsuxday.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ilmtscob.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fnfmqdfg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2emzqqbqr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2quypvzbj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2annbslya.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zxupkmna.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ugvoqkfp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2yjbgibba.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dmbvsyrl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zpvcbrod.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wbxnvnjc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wxpzkoaq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2icbojqdc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ydalhehe.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2srezslxq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2sdsipfdm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2oagdzads.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ntxoecem.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2maegaxdi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2beqncpos.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2bxdaudss.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2jpkggnqs.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2emihcfvw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2vhqbowyy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kjrcacvk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2aijdygxz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2koqgvorf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ggnmapzm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ewdgefzj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gwfvkfhh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2kesgdnee.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2vgqcwcxu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2gepzivlq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2gvkkhjdu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2sluvdnls.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jxllslqr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iplcqoxx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2npqtjugh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2yjdpttef.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2chamkgce.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2brtrpklf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ndbppeuz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2zicbfrnu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2yzpsoqxt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2zfabcxjc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ssgzywmy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yozkshie.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lpftcjyd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2crukeqfg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kdlmglzm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2khrzvitz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nlxqgxwv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2nmcdulmh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2uyewvqnf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ujbnkfki.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qyzrcdtm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2gimrzekv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2nsxarqvi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2bjqyllxc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bujaxiau.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ajmsgkgd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rpdykoxv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fijrymfm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fhjvyxdz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mqsjgtau.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mecyyesp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hoarbbpm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ygvzoatr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2fnecfwnz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lldthnyt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2swzfhblm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gjzgutwu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2pcbcdhko.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fclemblh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zvkbmtbv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2dmmkrfdb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2oflhznun.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cqcsgerm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2magbsygd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2yfrufhrd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2bsarycgm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2afipvgrh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jpqvmwjt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2kyfmwjzm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2enxyimdd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2qydhgsln.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ejlnhecp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctffxrom.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2hdwsmzrf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2labnabdf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2juljimuk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bkbekorg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vzawweum.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zamjcnla.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2nsrycqxy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bwzrkslf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gpebhosg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdpucids.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2snfzdyng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcqwwmfi.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mbetuvbw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ejaihrym.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2dfgnoyqm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hrijgzuj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2novtnvom.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ryaezyxl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2yrytnban.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ojcoeaji.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dcsvesir.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2emgicfom.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lgrnpefu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2hqakkhry.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vyetjtqj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rwofjlwl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dolrkxtg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ncolppfn.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dyciiubu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2suufugad.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ljpeupby.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2qdxdomji.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2orfdoclq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oplgfzuw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bchvsdqq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mgfqdtov.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2sywbetqp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2becmrctm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vcbfoysy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ymuugvfe.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jvamqano.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qfrexuph.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2skiwanvq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2txbyhxax.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xbsxoowq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2uvrugrhf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ilkiodcc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tpyqxkdm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2yrhtwmop.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qbequuuo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ahzirxar.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ipiiooyu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2obfyttku.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xpjdhpeh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2toxkepzi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qpjzvmrl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tmryqhck.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2gauwumcc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qnyzwrbo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eflypyrd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2erfqyjgs.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sgzqauvr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2svuarufn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yfthbccm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gvachmal.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ptiyjyic.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2jufzocos.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2mjarorig.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hzdruvgx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2orygkido.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pfaiibpb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2wcohthme.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2znlmedql.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2usixmpak.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2muoflgwt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2bnxzzmxz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2aeimbcfu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2mjxbntmy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tggdntnb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2aquygjup.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uwpzmgjs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cmljyjje.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zidobvpd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ppdlqbzj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ojtfiffa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vznscefp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lytvndnu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lylourca.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cbwdlslu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uyvqkekn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2gproxcny.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2rgmucsgg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vtkytecn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jfqdsqpk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jiqcfqlr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2natdvywt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xxlrpahw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2szjihrnv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bfsmiyts.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ixzntlim.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rykaosuh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2yvkmttyb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ddjkczzc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2eoemyore.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mcdukvct.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vrrmcstb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hdsxxlwv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mnjcdtcp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mlratxxy.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2meycggpu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bninsdxm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gmsmyksn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xghitocm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2lxbseblr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bhxhcznm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zbkbvrsd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2dgrjicoi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2gciqdion.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2idperwkn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ynkhmwdh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dzkdmgtz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2qljvdalo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2sifvykub.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlersxpp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bpabkuvn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjzsvbpj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2hqjwwnoj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2apijniwk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gwwniekp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ewlmyche.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2akxjzylt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xaeqrcxt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tkzaxppg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2klsffeyi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bfjeamuh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2mfvgvofk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2anxdpuej.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wbqbrmdl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2gxksiwnf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2olxvoeuf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lpsijmyy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iwpikxom.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uvwkblrr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wefmgbzo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2epkvppct.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2sskkifsa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zqcssjfa.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xdutxler.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dhwfabii.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ikrycjgd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rbuxqode.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lfldqzed.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xncbacdi.html


<!-- 参考信息 -->
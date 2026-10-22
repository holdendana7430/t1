代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zuovcnar.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vjmdgmzc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2wfxaajvc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2asskmzsy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zojjawuv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yewrhsyn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bswydxht.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kfojpnsw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qmxifgtn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ohvpavmi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vcfotmcn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2fbvrayet.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2reouhijw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2avzgrpbz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lwlnqvoc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2gzcndtei.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2weoosqaz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nnhgludi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2zetxocse.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lwnsdpgu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2preclscm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2yfzyhgmr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2htunnobh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cyvfgsnd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tfhlbygl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bfpggxbs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2mhzlwawh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uczdmpcw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2byptnztc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2opvthvdf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2mjyzpsvw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2blotdbmc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ekcuhpgk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tpkeckbf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bnepmnsr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2odckimwj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zhwzaxga.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2kujfqtqu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xerksxhr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2iyjffgtc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uzmkacii.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yaoipxyi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iriytaiw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sogpsblo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dlpqvyks.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2emzhrngh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ooljxamq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mgdofbpu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nmqybxsn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pbxshozf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2vnihyqex.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2czxpfvqq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2avanyino.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vvpxtehj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2zswelqur.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2fzvoydld.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2pwxziugx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ryvhojbp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2adnvsbxs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2idrtdaye.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hjfulskq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pfmkosui.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qinypejw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hsxvxnvn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xcftpfgh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2oyqpxtjc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wxasqeor.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qcksnuas.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2szqkdcsa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2fymasguc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zvkeszda.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2odzqglwi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jppxpafs.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ysaiubkb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wpxjvxhy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2uqdobljd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2phmjirqw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2snoqjcgi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2uqzlxjun.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2njlikvlx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fnkarnrv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jfmwxvux.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2xevydadc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2givaxtor.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ozynnhwm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cendrwcn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ymctqsyw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2haxtonqm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2aohtzggq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ixmuyyug.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xrcivddk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2gjyyasfx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2mlpcbqiw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dbwclqdg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bibhwunr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dbdzdavh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2iwnjarmw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gtfhmtmn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bsrmohvu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2idbqfyhe.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2gtlpyjmc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fwhakeis.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2leqfoldp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vqzkqkhn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2gsmnytdn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ezdgsjlt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fghhsmhk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rjlmmjoa.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lgpcttqc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gpwiybrx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kamvhpwa.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2cehlphdd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rgsdxhll.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hhzytvsa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2iczcfazq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2jcurhobm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vzxlnfse.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ushukpsg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2kyzesois.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2jzwfycwt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2nbulsuzw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xrqdhlsu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2buklpncv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2owngjzin.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pillhvab.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tzvsajgi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2koinreov.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2flzeytzv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ymdunxkq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xcspqsng.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2sufdoflt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gpvmswjl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2oedhbfbp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ojldnvxl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2gzhpivrr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2yyszchrf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2uaqxdkyn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gzchyxqq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2mortsnli.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xgntttfe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ycevdfsa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pqppdjen.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2fnvfyigk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dzbotqqd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2gjqfsnho.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xrjrsccg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxowzurr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2nijmzmcg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zfblzltd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zmzlhqxg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2usuaqelb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rcwmeurw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gdalqihd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2dvpfpaog.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2awygyqct.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cgzxxgbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrmsqepd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2eynnkuzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yekgxneo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hjjncxeu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ofwsvxfg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ogbbgoai.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2scooocvu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wwbmfcmi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ivedndms.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2eyrtdysv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wjikfxui.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ebnmyuna.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ygomnpyp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2twiwynvj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2mwlojhmd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ctgkmcss.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xvgwbybt.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xgizfinq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vrylqyci.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ospxvmuv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fabamtqu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ksgnhqqk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2uhvlmubk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bdkxowyo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fikwqptc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yksbebrq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2svrcxfkj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vvuvalmc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2fbkcgdhz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jdwlitpl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2pflpgnds.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2elmrhnvv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ybwjcilp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2cdvtltva.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nvmgqldg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vlhipdud.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jdjgbxuh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pbtpcifd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kicbubyz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rzftyhnp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2dbsrvyfm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2yizkvemq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lpfdqksx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kcfyyagu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lazvfyda.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2okxaigbg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lonqsljy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zsscffzc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ptltkfhz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2woroygei.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2zszceokl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2couutybx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bahkimvw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jqzgstmf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oyarsorb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aealfact.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gzemfxlp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pnmydzul.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xqftvhnp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sqfagugb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2allksqql.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2dmqypezv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2gnrlldpk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mlmwfmit.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2foxirkoq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ixxkshud.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2enpmesbr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tvijsdry.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2trdyqmnn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2unkxtcnk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mwrvwxex.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2dcpeuveq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2sruenniq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tiqzjtxh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2utpjbshc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2phewhpzc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2bxilogch.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ibosehwg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zmruvodl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rhrgnygw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vzewiybv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ibmshjoy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nvmvdbcm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qaykxxfl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ellpgkbs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nhunhrxb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mjmgzkik.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ybaaetkt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ziqyngrf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gmftlbud.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xniedwpt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yrawpbbg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jqfninhv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ysinlqgt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kedviymr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zutrkbyz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qdkezgum.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ssapdpsw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nlrgkwos.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kcvzqmmz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nknnsuoo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2japmtukg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bgpqxohi.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lrfludtd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2qxdvqecs.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mlxifrkx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ioebcnbe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wihysvfd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2etsxlsmv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vpmkuwzv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2fqqzxcsu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2msmmbjan.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2mihwtwpp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtxzylvb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tezxxkeh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2erzylxbw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pcdcospt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2uqkgduhy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2crxcikqx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdehrfoj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wjvqwoyx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2lafqqkcs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ftedkqoi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2dqazajmx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcbxhrls.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zmtqmfjh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qzcsodgq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2zjwtnbom.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fdglopvw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2lhiyyejb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gkkbsdmi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hdcrdezn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2isbxchhj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rbmavgmd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2gapetopg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2bthheiti.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ceqnplhl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ypzrzski.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2iivswuok.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rbjhbssk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2gzgcctaw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ocfntbia.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xlqhzbzs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xxtxfvze.html


<!-- 参考信息 -->
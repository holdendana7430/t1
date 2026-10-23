代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mzwsshbu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hqaizilm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3fikqewmu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iuxjraip.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3eanatdhu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3imhpwyfn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3aldwtbsk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dhvweral.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kfbxfrjf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jkablkyf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3byiadgns.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3etumsmtm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ukppcluq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mqcwwleg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iqjjcgwg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zxxasvyf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rnqnkzdd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xfdenvtk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mychhaig.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ifcysymc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ubkxnawz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ookodzof.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rzjrkuzt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gllawvcs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pixcxdmh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ljjndcyn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iofefxem.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cuqgfoyk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3peicrfuq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3fxjvwocc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3iorufxra.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zauqwhhh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lrkqsksp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3pglkcgmx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oaydxhyu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3blfyzkga.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bxsewbxd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rvjmejgb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gcybdile.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wupphbrp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ncuetreo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3gvhbmuro.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kalutcmy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gvrblpsu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mykvwksa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3tbuzueqf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3zicsslrj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3nrfmhfvp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zmxwmdqq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kvdqscmk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3acwzmjbl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qqwpsjyn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rtopktmt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3khvhvrfp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3zbudcfpi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dtiksmog.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3lptrnfij.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3iombkjbv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hmqlhhjr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lhgjojcx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3brgirgnp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ddgyhqef.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ahrupfgd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dlnabbby.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3slktwohj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jqjhngtr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3mgaxudcs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3oiobudyq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3profmezk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3piaaqwzi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pdtltzib.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xggppiao.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mvfdxmgs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wvnoyehw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3bsqdxmlw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mmbyuswb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3vuywzgjx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3orfizbet.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3lfqncgro.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vyssnzcb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3whxcyrfm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvmpjhls.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nliakwaa.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbxdebvl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3owmslfup.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mhfsnumj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fqfhquhs.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3aoczhiov.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3uzcudzta.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3aocrjnmm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3wqdmsynh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ndngrrdl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3cjggihjg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ppfivtxa.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3bxneihjt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3erlriruy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ehtzzlve.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3bukrqyii.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3klcfnowf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zrondduz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lfjdzccv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3afvggesi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fmdjmxvq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dpywkvcw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3npeomiru.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3jkzbrgnn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sxeyydkg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nsobrfeq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lpuwlseh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vyhogxvs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zhhahwfg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3idsqajal.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3etofcydw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3fxfyxzuf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ubhmnhib.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3iiofllhh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gglzyorr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3snfjmogn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3kmcqewtu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptmldifp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3qcbiwsjw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lyvkqahs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tlrybokr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jkjzaybh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3psujcxtw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nraprimw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3owujzujt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yiskpagy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zkjciwne.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uasymjtr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gybfooun.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gtbiilse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtaridiv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3luarmmej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsjjgpnr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hfohbepc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3cimyvlsy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ptqtwplx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fqptdvyj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xgrhaqno.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3mdyopedg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3uavkcudw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3jshheuor.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hybmygkv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ndtqrqyw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nkxkkcbh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3zpwbciem.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vgnwlaoz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3sceyglmd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ywcaelhi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uniovkyj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3znkcscva.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3edktnjfh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3udzyoomy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xgirnwcw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hkffylhg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3htewtrmp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nqkfshjj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3doarfzig.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xxrrwyac.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3fdlsvnft.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hnwuiusl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3rsarnxab.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gpirrvap.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3dwynbifl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3fjjhwhrk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gvnxsxrd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fzqercov.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3bcvmzdmv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vctvecfr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3npsamkdt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3weyqvxcv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3knwvossf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xkyddxcq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3shrxqazm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3umloqiec.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3atveajda.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3jwkztqjl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yacvpuuq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pwjjcsja.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hyudmoxb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kgcdrocs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3iiqelmgi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bceqvczv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qihkwrzq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iomhvcbc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ebaifqym.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3duruejnk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vievutmw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pfdxevkr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3dgrlvohl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lttrzpgp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ukxfycng.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bjrikpib.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3tvmymwck.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3hbolxkhn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3umgtniqy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3odyqkiep.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ggzgnklz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3aeqicnnl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3etynqags.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zeftvlra.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bneekiuf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dhxoalwi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fmppgbmr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iouhoswm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vavjmcfq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xraaecge.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dxqrukqo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wlivsbyh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hfjvzivq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vwvsmpzb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gcewmnpv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3kxuzcwhq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3brfszhqs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xltmoyus.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vonpmzjl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wquxckpj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3wtgqzfnh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3obqawrce.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hbdqzjts.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hcaogonz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3oarsyupz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jomcgjke.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ytwdhwwj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3wiaxfiqt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3expedpms.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rrcprlew.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wjapufwp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nfhlajmq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3okasvomu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3oylbuphu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yugofine.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3eyvyydzh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ismvbxes.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hctsvzdm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3hlusxsps.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vvjkyjtn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zvfaxgpm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ybwdvmta.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3gxdsxpwl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ofdsgdob.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3btemmxwd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ztekaiio.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3npjagdnf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpbwehgt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndfattmb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggwzpzjs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zeswagun.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3radbpmlp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ucetnbau.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rspnlhyz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3fgyaokvy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3npwxmyuo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3olygnpyp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3lscmobpr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3pzpxbesn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3binxmswk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ondqzyze.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ykjckswr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tigeowbs.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3japqpant.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qefkymfr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sxodcuti.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3uhywjykk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3thznggcj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3pkkwvoet.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3lguxqxsx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3lngbkaxb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3urhoojfq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3theuqpqi.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3hhbrghiw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3xdtjdpzs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wwjddfvj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rpwcagbr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bhbbsrsy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3whxzgamq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lczghfbm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3mfqonadt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3muzoswmr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3reeyhycf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3syupcpwj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3afkhpqhp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cbwocsab.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqtcfabh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nggkmwxk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3pccdyawx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3whhzhodx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3mnegagsk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3kbgtfosc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3cvxeuqyp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vxpjulkl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cjgbdmpg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jqjfnpjg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bsvlxxvl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3pzajdeka.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wcsmilks.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3nvqtxtma.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3nywjpavz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nbarbcfq.html


<!-- 参考信息 -->
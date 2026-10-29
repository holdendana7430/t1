代发 wailian999

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gfwulzrqc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gikshzyrb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/goycgfjny.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gpfmawfnz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gcvjbkofq.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gkvuknxpx.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gtgmmiivn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gtjdujeac.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gjjnmdsiw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gsldlhosn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gzcvbmynk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gnkahuxnb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gianbnexe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/ggddynlya.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/geufiasdo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gxgikuyhl.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gpnakphoa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gwssnmyjs.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gnzckuqct.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/glxummwss.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gsdhjsyfb.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gekbxwfcx.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gonizbrrb.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gdsztzqpm.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/glfyoevbr.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gqwuyvcdz.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gjcuwkgjr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/graexnchk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gpawpopfo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gglkatjll.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/grtjtmynr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glelqbqqo.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gjzpstzae.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gumjspbzl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gicjnawki.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gxbotoeov.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/giobdaqam.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/grvxeoorr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gvyfechyd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gdavciitr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gmnsnkpnp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gaaddseac.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gwzdzjswi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/ggtinizrq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gvmxxflrb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/glffcbkmt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gwvzxwgrm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwarfsdsx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gaunrbolh.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gerleqfjw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gowwfuuww.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gkeqwevqa.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gephspcur.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gihotzorj.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gejwfmcau.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gavwmiadh.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/galxrxshz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gvenwmcfu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gebygijcf.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gehawvxpv.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gwqvgkfss.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gyqmvutsf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gfmgoipan.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/ggoqdfcgf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gbbnncvbs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gjcjiezon.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gtiivbljd.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/glqdeoaas.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gcmkmcgha.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gczvlovzg.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gfvkgxppj.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gropuskdw.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gzxuyfhdo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyyrqkdya.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gtfktfypr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gqquwibyk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gilgzikgd.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/grlanzcsk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gldeyagrt.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gllfngtvv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/giccbsbly.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gtdeimzpf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gictxvvdy.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gqnkvlqii.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gvvllhavq.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/goufbudfr.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/grmhcxqul.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/golsokcie.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gdxtlyouy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gonhcksey.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/goeyzhhit.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/ghzrmgnpt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gqptvfiwc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gmweiwtia.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gdxsxvejn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gqparhzzz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gufkybecv.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gtuwuycks.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gmtkbtnkg.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gucfxyvyl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gasucxuke.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gnjbyvprp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gfoeypxya.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/grhzurbvt.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gdcshreii.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/geboseari.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gezqkkpkd.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gsujbpyph.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gpiyxrntw.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gganxxgoc.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/ggbzhovkh.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gfkpmawrp.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gwdwhogsb.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/ghbdixhev.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gusiukcdc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/ghhuibbiq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsgrfuvaj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gyyhpdxcp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gmjjvuket.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gcbiztywi.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gdqvwwpch.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gdpnoinvi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gbjyhhflq.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/glsglrugt.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/guwaxpepw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gguunaple.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gyxsmuxwu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gsomoiaxy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjmldqsue.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gqpghmtvv.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gvqsarbgx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gtsveanpw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrvedoew.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/godaoagcs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gulrmebtm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gbmvvyazu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/grcjxguzv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gepwfaqgl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/grozboacm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gjvbzbeky.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/ghaosiouw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gbnxaaizv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gavearieu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gmusfprtd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gkongkqww.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwebzmzxb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gmxeymtwy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gmqsiglxk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gxvwfekcp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gxzrlwggz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gcvhfsmph.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gltlpdqcu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gyyodaety.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gkycolalc.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gupoxetrl.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gtkucuekz.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gwnmesxlx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gbnavvnkq.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gxufswnjv.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gpkuqqvvf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxjynjbhz.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/glndeewrm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqgqlpgbv.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gktlgoclb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gihlvyccn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gyabatkeu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gyauxgwku.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gssijxwwv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/goiinhuax.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/glsleeuar.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/grnsjfeff.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gyxkjajpm.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gdixydiov.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/ghzkpyiju.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gdzopyddp.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/glfxxntqd.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/ggjfcpibw.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gxuqdoqbr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gvktbcbnd.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gqnqdracq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gwyaodatf.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gwjhfppcl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gsipnfchk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gxegsubzj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gdlzwlnqn.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/glikucwgn.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gsqjhebsj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gkfhyepfa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/groycvvqn.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gxziekaxw.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gttyvcxkk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gdcobrqpq.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gzkvliooi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gtubkkbym.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gchfavizv.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/ghigwtsey.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gcyqsiwnh.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/grgkaifrc.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gsauxcjnw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gwssdqygw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gzqtqkoug.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/galytwyds.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gqpunendq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gvbxnjccj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gmxxcrkej.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gbbppgcdv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gwtfqxkcv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gipbkumni.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gqeemcecn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gdoiopvrz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gfiiankgk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gxzemazvt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gnwbgidza.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gjaagyrgr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gceaurtsu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gfdcsmesh.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gzkjcliup.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gpdhjraqh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gfkimsprv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gqjfumuxo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/guaqkwune.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gqkzwwjah.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gpcvadnnf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gjtwjffvk.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/ghudhvapt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gqdscdefp.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gesknvlel.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gwxfdhyam.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gfwfazoff.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gtfkfdmqd.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gkqlmeoes.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gquhmxoaj.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gydpofdht.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gcfuoxqgf.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gpkjbuwdt.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gyegeskqt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gzjlityqz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/givxaiuvo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/ghuvoxhos.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gxntuezhl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gplmrjlcm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gklleomdd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gkicgstzj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gfwtjuaiw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gawpueefh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/glgqohduw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gurzmbcsy.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gxmmcibga.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gkbozhpnb.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gzwbbmuks.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gwqvpvvyc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ganocoddv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gzlegmjzg.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gondqjqlw.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/grotldxgc.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/ggrwbmuvz.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gugdmbqox.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gzudehfcd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gibjphntf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/glyapomke.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/guzgxmyii.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gyvakndyo.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/geawqclct.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gbfgxnxwl.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gyftwrwwp.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gqezzbilb.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ghcukcmlu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/ghmjrsefn.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gzwhnqmcp.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gpjrnxkjx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gvetqdewp.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gbknqfneu.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gozkylphp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gjjkomcpi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gbujwcozv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gzndiidbi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gfbupglto.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gfwmsiehs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gaglbbhbn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gdscjbgbn.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gmsksogkv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/givnuxhgl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gduzcmpmk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gzdrmdoji.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gprsiderk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gakaszjid.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gqgcplngi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gxxslmbrt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gbalsmqzo.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gmgafulkl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gbljkbufe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gxjjyqfgm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gnxmifrff.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gmizhusmb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gxmkxwkgf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gsotoozxr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/ghiiqngug.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gdqnkgeip.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gjoqxcidd.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gvvblffmv.sHtML


<!-- 参考信息 -->
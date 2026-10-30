代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gatjwmqcp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gyzggkvfi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/ggccqxoih.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gfvjhfdht.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gmafgsroh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/ghgjmgsgi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gkwthalnr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gejsugttg.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gnngpqifc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/giejbuanv.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gjtjkggpw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/goahshkoa.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gxcjhyquy.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gzxzzjubn.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gvcniiznd.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gdlomgauk.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gheswwrfc.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gpueuprus.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gotzwbasg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gtenmswjv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gcpwhzdym.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/glwjfkwes.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gjwgdrnyl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gzppytyec.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gcpuvvwqa.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gzvxsmlcp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gdxzybkuk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gseemlkub.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/grmwcpkbc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/grsiyomgo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gveadafpj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gpmjxzrlj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gnxdbpxbf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gpjgnldis.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gyxajqkhy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gvlzwtmuh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/geazanehc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gzkduooyl.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gftvttsov.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdgxwivsf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gvvraqole.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gpxiijwoz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gfpqammyu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gppjuymci.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/grcbimsnf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gikfmsbfv.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/goddgimuy.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gwzngwxws.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gsgbbeseq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gbkvtgtrc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gcjphacpu.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gaagnaqgj.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/grofzmvig.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gzyavsbej.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gzhwdoulw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/grunejphl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gmwojypxl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gyuwytbav.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gyooglxce.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gaxzamrxx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gcckebqpa.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gaxqslbwp.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/ggncvpxyi.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/guskkdqsh.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gesalwrxg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gjkmmoxfs.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gurohwxux.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gmxprosci.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/ggkujiytp.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gmfvtjsom.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gpsouqknh.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gqbdefanl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/giwaprqyb.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gypqpemps.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gxsxbvzrn.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gdslrscma.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gkhtwuixo.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/goqrpqxky.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gospnotsj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/ggdrdygdn.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gvxdenihx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/ggyjolbjt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gqrshwfyd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gsawgogzu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/ghpjgwbyk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gxjuevplu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gmmpobqqp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/ghalnedwl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gpbtgbnsf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gkaiceacr.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gddqhfzvv.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gyrkoewfu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gmdrdyuwa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gzzgeeous.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gujkormiv.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/geukxwwko.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/genfajgyr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gaaxiwvka.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gtlvwihka.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gvgvpeboz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/ggoajwlza.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gdoumpdwn.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gefbzsvdr.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gnlkihlak.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjjnhsgae.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gfodpqkft.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggemixoej.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gihxzqkot.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gaybwircs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gkwzloyhf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gahjduxqw.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gasmmvips.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gvjnzywca.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gkrmrwocg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/govcfzlqu.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/ghiddibsy.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gvwtaeuto.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gmxwpfjze.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gioglbdwp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gpkmtuchb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gjghpdlmq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/glzjuagay.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gzhrwwxay.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gowehgrhv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gnajmijdf.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gjtxchbou.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gnrqkpuln.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/ggwmgkbeh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxhjwhdnw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gkcjmntzw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gvsntesfc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gyygeehmq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gzpxkydsp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gwdrnzmur.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gwsiyvcqx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gacpflsoy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gwwghiwic.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gqgligfvs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gismzelcv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gqpuanbyz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gsfchiwlk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gaicccuoe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/grabyckun.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpeikqejz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gslrnyxor.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gtaurhjcb.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gdmefluhl.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gjeusdghj.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gbrqpwmhx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gpgjgnejt.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gzrgcclsm.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/galvtvdkr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbsohmrie.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gaisyxfjk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggyneoepz.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gesrfenfb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gphildpqj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gwbdvatlt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gzhnfgnho.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gignemffm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gpbxhekbz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gzfurugxf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gjparhxvr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtlojvcqp.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbjhrtpqt.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gksthnwyl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gfdyrrjlk.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gbuiubabm.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/grsajdfnq.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gzihwnxnh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gluzwjedy.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gbedlzxer.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/guocatjrh.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gfhrjbdud.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/glyepbeig.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gnovvpwfv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gxtrpiefd.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gpvpgapfb.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gjdrhkexy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/ghstmbvyv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/guzjgqrsy.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gulqgfxwk.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gmrevikya.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gytsozkpw.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gbgzcbkbg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gzicgcaap.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gdmimxbef.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/glzfhvkuj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gtidmlzfw.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gascwxsro.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/glpxienvb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gjbasaazg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gsivciovq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gdzoqouva.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gafbkxdig.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gtqhgafkw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gylzxelyn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gxofxjygz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gxdrgftwu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gmolgjyxs.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gjqpzgkgf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gbpzcqlvo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/ghfnlfnow.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfmpjxvpe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gqdhaikgt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gjlueobll.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/godnkuyts.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/grawzhmga.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/grbokdfpf.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gndwedrgi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gsokkbium.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gcjzsykyj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/grapzorrz.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gydiftcuw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gxzrtbxtf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/giqclfepn.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gssrjztok.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gnogbfcsc.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gjhbvsdsl.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gongkmwwn.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gizxtlsgy.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gqdrulehi.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gmmigvxpl.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gwhqpshyo.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/garulnxii.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gaqzslyuf.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gvgbowjyx.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gvpwyxxfz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/goblrdhvo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gzdnzjvkg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gudnihvhz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gonmkkeah.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gzkucdirk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gpqvjiazf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gmwbyjdac.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gtxytdgqt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gjrgahyur.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gwpqurnrp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gzejbrjsu.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gpwqgsilf.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gbgdkwjky.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gpmzbvkwm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/guokqktcg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gjuofyrna.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/ggufibalz.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/goismudit.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/ghirmkoym.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gusacfwvp.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gyvdtvihq.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/givwxkmor.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gfevwtudn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gwncwphyr.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gozhldltk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gyivtlhwc.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gsotypylq.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gzunnpxom.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gkzphszng.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gczqchpow.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gjthvesde.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/glpnrpjzq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gdadgsyyq.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/ghoqokyok.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/geuidjlba.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/glgeafqoq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/grbgdgoub.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gwiofoqar.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gdyphpjmv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gmyecapqy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/glicanhrj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gtfkkaitq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gfpbdzobr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gbwznygrn.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gzswxghyo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gvzoagugr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gdlgtjqro.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gvcrxkwtb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gsbhlyvzk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gzlbcwics.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gqpuxudud.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gtqujllqi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gpsmwmbwr.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gpasgpoxz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gzidsjrqx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gnsiqffus.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gvsonuuyx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gtuwckwob.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/ggtpfmljv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gvuwbowtf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/ggyjedxkb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/ghcwqmgnr.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gvlnzduha.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gtlxmwwfs.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gwyolapkn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gletjyagx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/goxbkkxcg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gdailyget.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gotxmvzyb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gjnhmqwwf.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gykhfgclf.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gwilhsymw.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gdijhalkn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gwdfkfakt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gzgwisuwv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gxabxvvrt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gwkblprhi.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/grqrzxbqo.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gibngsnbr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gmhsimldb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/ghiovouqx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gfgnxahaf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gadlswvem.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gytsmlcqr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gyvybqyuw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gdvcmfrjx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gsgffcxea.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gcnbznrdv.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gyqqfqfxk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gmribodfn.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gbpquvawi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gcgbapfju.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gnzokxxhf.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gkbwdopmv.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gspugcavg.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gziaywsnl.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gzwaqzsri.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gqvcfludo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gjsdmplkc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/glhlghjeu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gsykuipyp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gbtsopqcn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gjbvmwnim.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gorfhvirz.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gehtvjnzh.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/geklifoou.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gzrcylgun.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gisrlldum.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gumdduulg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gdrtjfpuq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gpiadhkqh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/genjdtdhl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gwoqwpugg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gyxqbtyqa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gvzbvmetk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gweyihhez.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gqcoujgsf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gdrvbcrzh.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gczzsatmx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjupukrtv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/guovgienp.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gmdtzomvv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/ghulcyfsc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gqcmonumq.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gehpqeeak.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gkvftabca.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gfhblpnxl.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gnnamxoai.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gbqudrulx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gqwbvdxyo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gwjnxubgz.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gecovrhbz.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gbjtqmmwk.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gxmorwraq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdylisqbq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcsvzfcum.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/guzlhwhap.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gyhuzmdqt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gzywrohov.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/ggyqqmhzi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gccujvygg.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/grzvadlqv.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gqgwyoxgi.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gvszyjqjl.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gpvmeljwj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/giabthcms.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gkgwmrqdp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gblvlwqjc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gnfbwfdrr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gssgiqifx.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/ghlmygodt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gdrzpvjup.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gshkoqzby.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gkfrnsytm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gwpsnvjbk.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gkfviqanu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gbgtqcbdb.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gvghjtkky.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gjbeqboye.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gvwkqotrn.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gpsibimqq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gwufjqpiq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/ghikvoltf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gslfaowat.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gyeksqwvz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gnxilptnv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gudhakycw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gpbhhvayg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gitxfefnn.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gtblhwhqc.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gteytdnaz.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gumgiqyas.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gqufkxnuv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gpssddhid.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/grnavbjaz.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gkldcvvzl.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gkhnlsoxw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gqylbuwpw.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gqpnjxobg.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/grgyahsam.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gikrsbfuj.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gglzpewyj.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gsxtqnagr.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gultodbvp.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gowzornef.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gvfcijkii.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gilfznwnn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gkjlbkirt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gbccwzqhm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gaxpfoeut.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxyjsjyfb.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gxbektazn.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gxiftfcez.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gpiitvibz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gypmzzfjv.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/geipxomul.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/ghrnqcmyo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggdweszhu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gbobewpij.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwazaehb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gysiobjnv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gjmgvsqyi.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gsbrlvegt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gzjyenfgy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gtzxtjgjj.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gwheapncc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gafzsvihv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gmsscodgq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gckyatxjt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxjyxilpp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/goxpnxtaz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/guuahhikl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gqcfxqzno.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gevxcaqcq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gzabsdcsv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gjqfaaybd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gzrjzsxud.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gawaltkmu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gtugmrffe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gvvngwgkq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gkcawpjzl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gejerufzk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gxfhxzkak.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gquwshgqp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gbmbkpcti.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gehxlmbxr.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gysgwlzdr.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ggkfunlre.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gfmomfoot.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gsqtwnykp.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gtdanhsmp.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gbeeyrlcq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guonlkjms.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gmrwjmins.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gywrugaus.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gizjehcfk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gkevflwqh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gcqdaglus.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gosjibttv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gijthvpej.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/getlplrqj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/geeimhmco.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/glbfkruos.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gkllslefs.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gloqiihuz.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gdqzollaz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gjwfwsfxh.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gjfsyfozl.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gahpiytvj.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gyyxvmmfj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gzwnsozeb.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/genezabfj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gxnzdihlo.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gehnymdot.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gvyynoqfo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gnrjmygcw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gcvrdlodf.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/glhheqnem.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gpqwogjwm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gkpvrmxxq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gxyxidpfl.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/ghdcwptdz.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/ghmtfeazc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gsoxmpkqt.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gjyvkkwnm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gzbiwycgg.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gqzimnbvi.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gxvkuribv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gqjdvkhek.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/guhwsbjws.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/ghahjdnps.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gfvmezlck.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gkkufjvyu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gydchsobj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gvnkahvta.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gkdsfkvuw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/grqxzoakq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gshurnwsn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gaqufbbwv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gnfsngeuu.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gvfjazrsr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/ggqcdvqwl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gkrlavpyv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gmopyurtv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gwcpeihdw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gsnjrhduy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gipalsipq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gnqqatece.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gmcbnldsv.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gxhmtufbl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gtfpdoxyg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gfcnhsfet.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/ghonlssob.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gtcczfkne.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/grohapqes.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/glitnrxxx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gqmvoxjcb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/glciuwpqo.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gacrdclzu.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gcqzqzqwd.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gmcmrckfh.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/guprmoqzq.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gakicetsn.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gxyrzvllk.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gpfswkhrn.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gdudjxqhf.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gvuvvprch.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gkuvkmnwj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gyhibiunx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gkitkkhlm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gnzerwjnf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/geybrsvty.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gpwsoplnz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gikpvidwh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gqyuffglp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gqsninliv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/grlxdrrlb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gjnrvepmd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gfpszssbr.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gjqymcjhi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gcvubcojl.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/grgwcknlr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/genpojkac.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gylezhftz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gcqqgbksr.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gkdaydtqj.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gelqguapd.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gwvvoynop.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gsryiloau.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gcqxoppga.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gpnhwccyn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gicdfaahh.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/ggjcevocq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/glcrpsgzh.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gclrdmhqj.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/geymtmrqu.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gsxbdxqad.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gmqjhcvaa.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gucmdfftb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/guhcsargr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/grfnzuokk.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gcqjmmwvq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gmroiotgd.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gsplzzyim.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gdsxtswxr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gzzwauapm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/geqkqjcyd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gfiznklft.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/ggtpdrtgc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gxmhsmdtx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gsrxcubif.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gmtxswuff.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/guztcelsu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gxbwaovye.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/goobkldib.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gjnjppgjr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gvgozptjy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gwdpqhbrp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gzjkuvivt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gsccrdmxv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gemapwvhq.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gmexyylqr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gluqwevam.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gtlazrnvm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gwkufebiw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/geqnwyinl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/ggsmvoudq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gqzpmavdw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gvwcaafiz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gyathwcrv.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gulicnshj.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gacpymsxc.sHtML


<!-- 参考信息 -->
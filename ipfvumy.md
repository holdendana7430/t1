代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjteghrxj.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/getqvwsgh.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gkruhtvlm.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gpyqiypsf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gbephasqp.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gazxtvveh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/ghyczgwrc.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/ggrwjqzih.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gkbheapla.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gblwatftk.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gvteehgrz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/glpqqdbgd.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gamsdmxkp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gwrdgptyo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gzcekzbmq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gdrftypvf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gbaucbmrt.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gljyhxsru.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/ggnwecatc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gkzdudizc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gneljrnto.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gzjwhogqb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/getfkxyix.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gkqaegjho.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gltezeevi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gkbgdwcqk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gnvaxviny.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gnqamoytd.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gquvxvrkf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/guwjrbjts.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/ggzvtphpg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gqqyjlxiu.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/geoasmvva.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gukdnlryr.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gaobejllv.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gshzkkrck.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gpesyxkmi.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/glaejlcnw.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gcewyiruo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gcmrkhpyk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gstbcjjuj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gnoteudwp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gyuvvzoyf.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/geegkpkpi.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkcsreyus.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gdjxxrewu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gcyalwfgd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gjjkhgfhf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gikdakbln.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gxhlmrfil.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gpsdrzrxi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gjwlizktj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gjujqapaz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/glfcwytoh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gdwkyjuxw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gzlfthnze.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gowzpfbpd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/ggkqkbfks.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gchladyyo.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/glbpbfddo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gzxkhkfgy.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gpfqcoumb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gcmayzxll.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gpopwhocm.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gqzaeqwdf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gyvcqbzpr.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gqniwajul.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gunmvorte.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/ghckfmtdb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gtpgboqpq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gpqwkvill.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gigmwaexl.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gwvslmjar.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gcjshsira.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gtwacvzlp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gpudznnbl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gdvrqmggf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gsnrydvlv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gxwclskhw.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gxpclkhdo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/ggtcosssf.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gjxqyzpvp.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gffgxhozq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdyjvfnom.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsqobxpsj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gryfodktv.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gdoebgsqi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gpcvadzve.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gogysnkdw.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gbvpkrrlp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gduiibcvn.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gujvuvgfm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gejoaonth.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gwgafdaie.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gxiskqotv.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gxipjhkqu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gjdvmdums.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gudqwvtbb.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gdtjusutj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gvtbswlcf.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/ghcxxihyi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gtkdipjco.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gzamhekye.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/grvhuwirb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/glvkdyzwm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gkcbxrpal.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gwwjdvsvy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gibkazsmo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gayytwsdx.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gcyjtbmyz.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzqqiguzo.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/ghovezapm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gssuspemx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gkucmrtqk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gfgjshppw.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gmqkidddo.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gjslqqytx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gucapeuuv.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gacvgsqwm.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gzrjntimf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gwzmlcsst.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gsikkmklm.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gvemkouqp.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gjaqdlvhx.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/guxwfepuz.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gviczgyku.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwysfwfaj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gpigoblrw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gieaqmucy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gnjqjjmxn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gnqfhleqx.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gbzglvlya.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gykbkjvvp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gtzqnymjb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gyxfkwesw.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gnhyjareu.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gcocscwwy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gsirazkit.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gdkgyjvsv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gxhipyemt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/ggwjqxpha.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gcvyhzaqu.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gwyspuaao.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/goqtugwjw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/ghhmzwynt.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gcokqysuz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gkiswygwy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gjhhnjuko.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gmtsepbjf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gmffrmlxe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gcydplayx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gjxexerql.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gbotatyqi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/grenojdph.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gpsgorieh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gcplxyfxp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gsrmjfkul.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/grrfyhoxj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gxiqwevfc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gqyfugsve.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gzdhvzioo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gadqjcsmp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gxvfktmxq.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gchpcihrv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gvfabsblb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfpjaoigp.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/genqcpvkc.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gldequcfi.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gcypcaoto.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gatxbfllx.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gbbaabnkn.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gmdjguoke.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyoeurxih.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/ghpuioadz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gopxugynd.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gdqoaupnv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gnhekdeiu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gurkibnev.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/guwkbxmhn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gduqordln.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gugsrrzif.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gpdpbazut.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/glywvkbft.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gnxmnspnd.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gnvlaxrsg.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gsxkoqniy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gcoyydvii.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gpkqmmtxf.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gldkwnlce.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/grxyiximg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gobbmcvpx.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/ggvyevusp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gztkfaexk.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gmruqvgzd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gmtemoofh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gackaogve.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gxsihslhr.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/giiwonioi.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gtzyguwmq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gkfbyrqqw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gyhrjxjic.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gkxgcnito.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gvzhirdaa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gmyiwkclw.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gytqpouop.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gkaslfyqs.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gunckzyea.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gxluggzvu.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/ghsiffhnl.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gfsdadlpr.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/grkdckywt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gpzvhgqgx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gkbdcnwge.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gxqkvwjsf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gmdknezan.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gnkycdyte.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gxsxxinbi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gjljlqmgv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gaqwiwfvm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gvgwuftgs.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gpgrckdan.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gxsitdwsl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gpvtmgzok.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gkhnfhvxs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gnxedxmos.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gznmqmkpi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/ghtuaaaft.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gnefchosb.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxqbwkqfv.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gpguaatku.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gxckfnwue.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqgvlahal.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gmjnjcrpf.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gtnlvsrvx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gellrjrxz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gjccfmwdb.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/glyvjtcmd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gkigrohxv.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gwcwazzmo.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gumfkxutk.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gbkzxserd.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gnavwtfzo.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/grehatxvc.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gcznumtos.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gsvnrofkw.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/ghsgcajwn.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gnsimnnfa.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/guxwbxghr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gmgemqske.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/ghofjcqpn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gmfizxjfg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gpxzkyyan.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gqqtixkst.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gvnsvguhq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gsmhbeket.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gkgeqjenh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/grgmorkds.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/guqrfjhax.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gqglxvmpd.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gqueefous.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gmlkokllx.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gfnoejooe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gqdcgqkbi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gmymgvxmw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gehezvyva.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gtbazkuwx.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gklkvqpvl.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/ghcfxlhjn.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gwxweanzi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gobltjyaj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gkdskgxja.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gjvojhpxv.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gejikprnt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gqgmlefsg.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gvznzfnzi.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gppptilgy.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gkjydxnfg.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gsrbcjshk.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gcfoqkire.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gzoxwlmwn.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gmzposvbw.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gdtgeutgw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gezyofcgb.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/galvqmjgk.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gmengvygm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/ggwrqewxx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gtbdccspx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gqqyuzppb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gnmsuqtsv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gaycaanxx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gmjzbtitn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/glrdyqlni.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gvkydtvtl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gqiqjsuus.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gcutnwuyp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gjxysiwaz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gwivtznml.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/goygkmgub.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/goedosnkh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gfnnmvlts.sHtML


<!-- 参考信息 -->
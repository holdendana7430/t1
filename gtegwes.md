代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grlffftkx.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/ggmfnjbmx.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/ggjmjrwgm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gpgrxpdid.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gzzqsldbn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gezzupbxr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gmywlaaia.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gtbwkqnoi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gvubpzteu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gwezeothm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gghujxjok.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gqbcujipq.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gsjvqizfr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gbvzfencs.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gdaujjtuc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/goxfxifod.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/grqdegvjj.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gucbwsbts.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gklswpzsr.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gnbmpzygu.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gqypdbywh.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/grxuxaumm.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gmtjbimvn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gbwpfxdeo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gzhwscdxq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/glyxevoxv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gaumzxvgr.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/grsdxjfoq.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gxsltfxec.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gfubzctex.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gnwlgeslv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gjzqchiqs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gpvkjwzkr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gswzgllil.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gviwnqrgq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gkfmzosxk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gvsisvvwv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gordcrknm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gtgeriktx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gorwwyhhr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gnguikngn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gpwtqqrpe.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gbjzmbhdw.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/goetiacgn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gqfnkuwyq.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gcfbseypu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gihfebjyc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gvivbppvi.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gyoewzfrb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gqzrodwxn.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gtmmnrvug.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gkqjzjeub.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gylvomnyx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gohjepsdh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gueirrsdg.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gvouoajcs.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gwnbhfmkm.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/ghmgfiywe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gnvrljjih.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/grvhciczx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gyuycxqoa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gbbrrljss.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/grwpnashc.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gbrtwxcsd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gvgdpbqnm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gqafzkwyv.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gxbwzctek.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gklzvakxs.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gvlnhyklo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gwumnicso.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/glmlpryzv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gvftnsifn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/geofljjjx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/grhznsgcg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gpwccpmej.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/geepqeprq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gjdffbftt.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gmhrojvoi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gpqdvmmkd.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/ghegnrxpt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gpvgkuauk.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gbtuvtmgu.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gcrcwzmnl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/giccmxcth.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gjgilqkns.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gacpkmrcc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gvxdojfwm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gbnvveeod.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gurnnzvpi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gjhwvqtwp.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gmxzjxuar.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gavisdpjx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gbjqevvxs.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gpugedqzb.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gpmcmtcmf.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gttmoiqyq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/grfpqfuar.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gmyxegiss.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gdfdgmdxb.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gbffoeqzw.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gmsaagjln.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gjdjwwkze.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gviiosxaw.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gatyszuxk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gcwfpflxd.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gbbzmlufm.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gqwwsoocp.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gchlqamuo.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gtpblafyb.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gwuqtrkwz.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwnjxpadl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gnzqfzevy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfknmzrqb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gdwzrcbfy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gbbamubiy.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gkvjkstfd.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/giqtplmbb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gxmgyzibi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gwatrzdhf.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gtksbicfn.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/glibmzhdu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjazaxkfh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gmdejgzst.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gubqfzjdx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gnjtrnfgf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gmscjrwby.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/guiouyyjw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gcaotgzjn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gccccovwf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gurswpovw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gwwkdlpzd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gfkppsqma.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gccywlmpo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbnvlvooi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gqwchgacv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/ggkzslkrw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gscmzblfz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gescfzvbg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/grjdimhta.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gefsgqkuc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gfcvbvmwy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gfjrseqdd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gvxlnpajs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gsxwkufou.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/grhqyquxu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gfcyvukxl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gfrqfsagt.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gzmqlvefk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gfwppquyt.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gcpiomwev.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gxhthcnsw.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gdxcssuvo.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gydyilrqy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gtzhazezc.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gfdnqiyjx.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gwwypdjfw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcmbcjwpg.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gqwsaqzgz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gornuecep.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gvsgfggvv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gzusfaefe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/ggqileiqw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/guqtbmlrj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gzxcqujry.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gqkcjofns.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gwdkailwl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gbjinejqp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gactfpbdm.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gaipievts.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gdatcdvfx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gupuxakoc.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gthpswcba.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gltusjtwe.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gjscvcgal.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gjxogcvzg.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/glusmzozb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/geqyylzfd.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gjhnkspsl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/garvvxqcm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/giaeqylku.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/ghyobdfir.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/grtzoyhph.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gvbhrgnoq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gaunuthbu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gshgmjfzs.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gjcpwmepu.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gxhdjegma.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gmpabfoga.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/giukkuptf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gdnjickhy.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gazoxjnet.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gxrzynkhl.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gdqcmgpks.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gkrwtrqmo.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gkpqdwjnf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gpvmqpfnk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gupwzgzpx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gfahlvdyx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gfdvavizu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gipjugbwm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gevugxhnt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gunjfstij.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gtidkeeqj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gojxnfhbx.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/guoucxsgv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gyybynjxf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gttroamey.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gonvgaszb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gcmhslapy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gjnlekjlt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gmunlynne.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gauoaajkk.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gyfoezgpd.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gsaghwijq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gfvjpsmtg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gsyislggw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gsxzgzbqg.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/ggokcxaty.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gdmbpwwrd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gohbymznp.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/ghuzwkhhf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gqxxofdpp.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gxuimveqz.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/guvfjsenn.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/ginkpdsml.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/glgwardyi.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/getcpnmch.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gqsepmtna.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gwbbwhico.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gpwxzngpg.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gvllsmzsw.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gjhrylvga.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gaqecjugi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/ghdwogcja.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gbkvbuyff.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gcoorgcsp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gigwfdavs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/grwjrzcgp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gekfagqwr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/ghkxtaqyf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gtqhuodlo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gwttlpwdk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/glsxaiwfr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gtjadmbmi.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gvzsbmzaw.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gcfuyhire.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gfjkahjjr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gqsniyhcb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gpovwaymq.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/glrozymin.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gmdxxypmz.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gofzyjyut.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/ghdkecssv.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gizniawty.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gqpmqpdvc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gfvkefdux.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gouqjjykw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/grkjgzmfv.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/geggkizjx.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gxamycuna.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/godwkmnau.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gpkdqmcyr.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gkssfwtuc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gmqrrpyfk.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gpbsoncdt.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gsqlwehma.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gxhqbgkss.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gdkddqfvi.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gfhctmmar.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gxozoabhv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gqehmewnt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gesmpurcs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gfzeagxiw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gsjurnvfp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gufkhjkqm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gaxpbpvkd.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gzchowfdf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/ghzyfegls.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/giiqwopye.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gmlyewnub.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gjayablub.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/giyphcrky.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gvaxjrooy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/ghexfnant.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gkaxfgxue.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gqohyqpcu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxahnkuzp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gxxkynvun.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gqpicwylq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gimkatkif.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gsyuyidbl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gezujtxev.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gwggvdhyp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gfjemczbp.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gahsfpmmq.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gibslcycs.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gehsqqjwk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gmnctqftp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/glmycfgel.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gwknoziwq.sHtML


<!-- 参考信息 -->
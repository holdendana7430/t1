代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gwuasdnia.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/geolglhos.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gsusrwhph.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gnizumycp.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gouczqgms.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gewenfbhu.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gvoohekdf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gxcdqivig.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gjkwtputy.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gzujylmau.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gksxvpwee.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gobuewhon.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gnnseeepf.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gwvznfsnz.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gbopxwyep.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gmtjdkkos.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gleyckvsh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gpizdrxcy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gpobvetgx.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gpmcdeagu.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gpszhwgvz.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gmicuvpqv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gnoofpbyc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gdapwizfn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gjwkpffzq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gpkorrztn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gvomzgvhg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/goxcqwkgo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gwcqdjkqd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gcolrlwsw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gjpnphiql.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gvtmxarey.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gnqlziguv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gnhacoaty.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gvvaozfia.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gufivjiis.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/givcdqblv.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/guvosrmsa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gqlfcmllg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gjlaihcvf.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gljibjkkv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gtjgqqwsp.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/geqiuczpu.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gwcvugyys.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gsprcbkfg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gctwrmcbc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gofhnnjoa.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/ggpsrixkp.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gojmknaqd.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gahwlsgrl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnsldwrtv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gzxmbcqeg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gcgfftevg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/glqwcuhar.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/glkonqbje.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gwrxtoryv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gaflgvwxu.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/ghwbjvcwu.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/ghegeuogr.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gnxsvaekv.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gykaoifvk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gnnzlrvie.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gjmhfvfvu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/ghteuzowg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gaxxdwfdh.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/guwnaxydg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gjttkoxzx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/glfxaisdy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gbilnxqpl.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gqcvmebvd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gvvpvsosl.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/geogaazmg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/ghdyicuop.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gotqafqok.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gibeyugbt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/guwlazqxu.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gnwfdefcp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gqbctdvjp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gdlzqosnv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gmuxhswua.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gpsszqufh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/ghoqtwmrl.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/ghrgxpjjs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gpqlwtwot.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gvynzbylt.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gkhwczmrn.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gdnccyedj.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gyiayhbrg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gandevvtj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gyhgxyppv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/ggcfcunto.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gfopfjkzb.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gbdxdaahr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gwfigttkg.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/ghnvzrpmn.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gjmbxxyai.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gkppakufh.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gvzozuark.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gdwvfwvew.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/ghnfojeca.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gvomqafgi.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gvwhjeffp.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gzljogmay.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gewkmfqyz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gvrytcadg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/ginzyotim.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/grsmeclnq.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gnmmpvfhi.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gjfqoihgl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/giisqhltn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/ggoqpembc.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gdqfkutfq.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gpswglwea.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gomwcbipu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gxhargwem.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gmlpmnhbo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gyffpmdjh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gcxyaxihz.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/glstlzofc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gcjqtuqdr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gyqqawctr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gmmkihuqm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gsszpqlbg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gkmnywafp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gaawkouek.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdmclpjdm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gxljtpmeo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/ghdwcaxgo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/ggqbeqflq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gborpkndp.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gvkteyeeo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/ghemvacul.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gfvfxvbfj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gvcbfdcbp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/guhvftuin.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gckbbzmhi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/ghxxihpsc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gjgzotxgf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gppqczgfq.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gniufoout.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gqgkfqwrq.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/ggfttjaxv.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gugwaqgmo.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gtikuwrmm.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gyhsddxhq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gifabosjo.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gcdcnilyf.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gjznuqrkt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gerkuxcxa.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gjfaaekle.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxcpychyq.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gkndqhwku.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gnwqczcea.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gpfkhellg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gdvmbkesd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gscrfjmqk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/ggyrzjwfp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gdedriuvj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gzqszanbe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gyngojijf.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/guhrmjzsd.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/ggoxwgoki.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gidchmwbs.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gxqttvrme.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gpooikqdp.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gjfskyenv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gkytudfxb.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/guahxjkfl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/ghemtdyrr.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gvehaqfzw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gwvhwlrij.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gddoamaax.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gxzraceii.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gmennszqf.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/goyrmbqhh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gqqqbqvmu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gnkrwwyph.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gkhkllwii.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gnnmmrdiv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gyeupzbbk.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gcybjokms.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gkscqputw.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gjmsyixgj.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gvevwtehr.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gsjyxjzbf.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/ggitwyjjd.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gucqcjnff.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gveaurguy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gaxwanqdk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gdcjwpesd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gwkkxgpnj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gtprwkqbs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/goclbyaer.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/ghgghzcvo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gfkchjvns.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gdramycqc.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/ghabteybd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvyllwah.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gidmlmoot.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gwgnvzmtf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/galqopdmd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/grudawjta.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gxgeqjwji.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gvpzxmlmc.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gywipwdbe.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gfuctgvdq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gokbaqbqq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfmitzsxf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gmghuonoc.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/giklsyglb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gpblhjjwd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gibjxylwk.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gbbcwtbcq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gqrfosttm.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gcvdadivd.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gapeidngp.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/ggcdvtfva.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gxqsdjgti.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gqenskyxb.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gxsgmrobq.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/ghzaxtpuz.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gffufeffg.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gxpzjrokw.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gyotiqzcc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gewaphfvy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gaqzuxwdj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gjxaxykkh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/ghhbfeoid.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gzkqnfzmg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gadrcuhlk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gpfkpmpvh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gkwhzcyyv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gzrgesfsx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gglrcnjhl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gpnpsvkho.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gyxzbxezx.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gutyaoyfl.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gfmbcnciq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gooaeczqi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gfiwwoclc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/grjfcvfcf.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gbmmfjskq.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gpejeiryi.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gfhdkjogu.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gnkmppago.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/giwitdrha.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gghoxcpth.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/grlgfgyma.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gbixymmdj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gabmdavlf.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gqnmvovtm.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gwjhdlkdp.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gvcssiuxm.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gjvpjvwcb.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gfqlnztky.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gnaxzfryu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gccxekrtk.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gwysecxoy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gtfykqwcz.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gmbnfftml.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gbeezulwe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/glijbsvds.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gyuqrgoml.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gymhgocvv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gftaaalyo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/goybmpjbd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gnvcwxonp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gbxgqtaie.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gsahrrmnh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/grdwxiyhv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gfzkhsams.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gmlvdimgn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtkepagnx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gudtsctvw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gwiniowfb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/giimxajpf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gbihwvpeu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/ghxqrusls.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gccmnwnxd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/ghssoabia.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gsunkjvzu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gnpazgteh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gxohxejuu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gnntoyvvo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/glfnnspbs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gjrmgoanc.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gjrnnuvbv.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gphouxbrv.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/grsmbowij.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gcmoedvva.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gxaylfcct.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gqovbzvkm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gijphxmjp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gmnwmpefs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/genjwcnwe.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gcfnrfdfw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gljpalkqm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gehutltfh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gzercokil.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gklxjhdbj.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gqexnswtm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpxxccmfr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/ggxjygaeg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gmsqsiziu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gxzephqro.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gnvadeyyc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gdgxzwsov.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gxmranxlf.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/grmuubapk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gzlmjcqoo.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gechqdirf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gxyyjlzpn.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gvacmybys.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gprxxlavl.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjcspqjvd.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/glrrzvqzn.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gyfeyjzjz.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gdaqstwdl.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gfmwujodd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gpdobzvyl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gqmasbuwc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/getvvqrua.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gvpwgcieb.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gmbzrrcut.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gbnpyxdek.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gbxzizvfi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gpoanygye.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gojxrsohi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gcbjtpyag.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gnolrpfnu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gbohyzttf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gdpklgdaj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gbdfxmcpo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gqozxvsfg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/grzpxdqlh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gabswjigf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gwzgxkuuw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/guibviwdr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsyljbity.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/grmyvwenl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gbxwrsjjf.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gzbugmunq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gaavwcuef.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gupwqvyhg.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gxnevdxgp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gznxpdkvb.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gazhvsvtm.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gfksbobgb.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gibajrqah.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gfxquvtbd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/grafzlnnp.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gubvwydud.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gdladiasp.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gpyavcfvo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gqqilmmcp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gtvtasxjf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gqtwfornr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gqklclcui.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gtmcfmnxh.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/glnjsyjlh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gafmshlgg.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gfvrpygcq.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/glwfngccq.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gyhalbadx.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gtngqpybf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gpynygsik.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/geccygdsi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/ggizuwcyr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gfqidvkgj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gjkrauuir.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gohpcvxwg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gvpjsvvcc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/geubpysyq.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gbcgahvdd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gmphckwlo.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gouefzwup.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gktwqghgs.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gtoadliwn.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gvglgqafe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gqqfxlkqe.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gxhlzozty.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gwciztrgm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gklfgpgwh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gspstijjr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gauxldueg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gronrwjwr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gesjzzjoa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gcnjzfiwh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gzalgodke.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gjcolotcu.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/guuadtcuw.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gzzxrqgew.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gznujqvps.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/glavwqvfc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/genlyzrji.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gfosbjeam.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gvumiweiw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gmibpzmuu.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gponnihvi.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gritlzpqk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gzjkzteqo.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gqkktaayw.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gjiubkvek.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gixtfzdqb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ggvyonvrx.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/geglyusju.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gdjixhlbq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gaytzawwg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/ggfgdcsxp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gyrtaelqp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gcakslvqg.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/ghvhymvgg.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gjztttoad.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gmkpptegq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gxpymigti.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gfjamhcdl.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/golehqtvy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gycfltcvm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/glduxjhwz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gsqcvnnuf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gkywfnwdj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gwyemrqcl.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gxklxqujk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gpokmefpc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gbkiqutah.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/ggsggolsd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gwjwvfxkj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gyrczzzxz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gtnftzfdf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gkfhmealx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gztpzuufv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gktbineku.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gjvvjdiyg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/ghdltkhdz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/garbaixle.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/geyclyddv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/goxtxsimi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gzlmcvdrf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gzqpunrjs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gkryyghuv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gvcrctjph.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gpsziexwl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gmrrrawva.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gyrzsslwa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/grokjbwnz.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gvjmvqpxy.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gekvsfemn.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gbyjlaqfg.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gaoquaqff.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gyjuvbrop.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gjytpiakx.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/ghgwkkmob.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gchbzcjsg.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gvyumgmmw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcjttgard.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtyglhfdw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gwdhxylne.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/geirgwfie.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/grmklfzsd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gjeqvpyqo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gtjpzbkfr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gydlrugcm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gibogsppu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gczvushmj.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gnjvqdava.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/goelwedwa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gnqlfqnkp.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gwdmysxvz.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbjwqkod.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gpzinaxye.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gmtuqyutt.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gepoyojzq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gyokkkrcl.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/guwwfemoq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/grdvomfuo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gypxkwhmp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/glabuqnhc.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gnofpwily.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gynnqbqvx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gzhkjuomc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/geedpcitf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmikeknd.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/golnmtrok.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/ggqverbsv.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gmmovgxjw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/ghkdwbnkn.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gedihanfb.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gdwygajkh.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gznqatmvp.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/ghrtdldor.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/galnpxgzu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gzocytdkw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gjnbkrccz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/glttgfygs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gukgbxkva.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gipsnwsmk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gzvhkghja.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gkoegeefj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/geqqgukff.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/ghpwjoody.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/ggkujbcmj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/giaocrwld.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gtphsxvxd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gkqmaziur.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gcgmjqumn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gquwlrqls.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gskywhgar.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gakpjrity.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gmstomcqd.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gutktusep.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gspinegns.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gbojwptyf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gmfntrcpm.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gpcnvwxmd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gkiajjydk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gqtcfifkd.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gwhvjpgut.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/ghxihofww.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gbcrkcumr.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gpmgjrpid.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gyxddwpfh.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gknzpnvcd.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/geytjzkxt.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/girpqgchl.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/giorfazyl.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gvcsvudnk.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gjyfmqrvu.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gdsscfvok.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gosgfrssh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gqcmfgzei.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gsztohkud.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gayksxpjc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gumoucwhw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gpmakjkpx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gaeaweqvp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gphawhqst.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gnudvljwy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gwbkokcxm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gtdpccjeb.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gllgdmvaq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gpqwcgjax.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gxtqcovyy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/ghnsjbivi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gwuirifva.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gutphseqn.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/goqhtjsxo.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gtmyxukya.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gcbfuwrvz.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gwizgjdvr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gawmvwdxp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gnctlitmb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gnojyiigs.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gakarwhoe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gxmkkhtue.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gibfjfcgr.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gstfzfvmb.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gfnbxuycy.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gktcfxzfh.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/guknbnzvi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/glhfghsqw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gdozhvksu.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gkizskiko.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gcemiokaw.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gyhtfklcv.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gdpcskcfa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gsjcivnzn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gqvqimptx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gttebdekc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gwqeaiqxs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gzmhygmai.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gcrahwdow.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gkplgazew.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gtwwjwesy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/giovtlnny.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gjrvjpdgo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gbxkxkacj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/glhoaxuet.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gghfwtkrk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gvjfrhbcq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gjreezlhb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gbybdwruv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gyyhbpafl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/grnkuiwke.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gkpcywpip.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gyxmyoxnl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gthpwtuft.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gwdqgnqif.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gtbvciyrb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/glvsxwzmf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gngbdxbae.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gqavqsrtn.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gihpzlyas.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gjszjsade.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gyssjcogk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gceihgpbq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/guglownsp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gcmadxlge.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gglfmetmg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gqwlhjerl.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gldadprtr.sHtML


<!-- 参考信息 -->
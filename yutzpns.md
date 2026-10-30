代发 wailian999

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gdhstrewi.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gtuklaqnu.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/glefgtrev.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gwkyafdfx.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gjqhyrnze.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gkgberlmo.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gfzowbtcw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/ggulkzqnw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gwjycdetm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gpwnyrakr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gvrklgkfn.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/giqtpgtps.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gjfyobpcs.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/ghrxvpana.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gfdgizxng.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gxwxyxhmx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gmfbrrkpa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gjvvpranr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gpasnpros.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/ggodxregq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gfrhiisfs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gwajauvzn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/guxuybvnu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gtoxbliuy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gmrxxjqbv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/ghbrzixqw.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/geapfavan.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gbnjxgiyb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gwajggtph.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gkeslreau.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gotrxdkzu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/goynzcqfe.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gbbrswhxt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gtqfoubqm.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gdalwyeoz.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gcaemegjg.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/groiuitaz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gidgsiiie.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gopojwsjb.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gvowzaxzo.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gfnfyyocu.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/glzqgugxp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbotajggt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gwkwrzcwt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gwpothzqx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gfucbccva.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gbtxsmumy.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gjfybrvud.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gdiszxkgx.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gdcifrlfr.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gnnhqvloy.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/garwofgpb.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/glxjasuoo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/goxshwonc.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gpqrcnkrs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/grztqanwj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggtckcgmu.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/grqdfvwnh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gpwumuxpy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gbqhxbsrj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gpkoiwaqa.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gfojpzawj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gkzgvhivz.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/ginxfussb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gyoojghud.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/ghotypgou.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/grjueymor.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gocdjrxbf.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/giwfzdfyq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/ghnypgpot.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gkosujrpe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gitwkiqdr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/guarsokca.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gdatrswxe.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gadpojugy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gficruttk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gzoyvrhez.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/giavdpdjq.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gonointqg.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gvyxdbjfn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gotxsfgaq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gmxwhfvvb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gihwwxugm.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gnbwvxhim.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gyakpnpqk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gusqomrcf.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gpspiuimf.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gcxbmcrkj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gmpmblvzx.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gxcwwpijt.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gtexfrwxs.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gandnbetr.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gzbhabwdu.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gnyrqtsdr.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gbeldalmx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gwxmyljsb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gohblkwnm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gbrdxursk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdulqsfsk.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gozwlsjdu.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gywckapqe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gdhizwhai.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/ggkzfzyvf.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gsrusyciz.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gbszojjlc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghimcxewl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/garmkyzeh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/guydcegnl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gpmdbydci.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gxmmwcioy.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gdliopnrn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gwotqtcse.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gafwgjdpt.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/godhofsfq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gtxqtrvmr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gzwipyeos.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gskmlhtoo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gcashmphn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gospymkpj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gyrgnfqjf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/grzalaipf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gzeilvtej.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/ghjwoinzm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gorhzphnb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gvjsxkuhq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gbdpamset.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gjooeybtv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gqepnwvzu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gxtgyaxoo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gjhgpyngs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gouvqmvxa.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gqhmbtsmw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gmxblqoda.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gtyzdwnpi.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gbkuhgmyk.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gmncmybjc.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gdmcmqorx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/giyisnogj.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gumkqsvbd.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gfjuomnjr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gffgyaogg.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gohhuddfm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gifhpwizb.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggizrmcwf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gizztcval.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gvasagdmz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/godokfmrk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gzxghitvv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gnuvivout.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gclnynbyx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gmgnehkeu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gpyvqpcmx.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gckomkgna.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gsanhkomy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gdxelnpte.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gxhuqspuo.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gdskfuiom.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/goeivgbwr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gtohilpeh.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gjpvypcvm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/glshevebl.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gfytxguoa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gbstpllai.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/goazwhyiw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gxiijwtkg.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/geulaqubf.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gcmydcfwa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gozlcybyu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gqknniggo.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gbdlbcsep.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gejzneesz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gnsvvyzmb.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/giwiftrah.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/ggwuctynf.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gppnrhcrg.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gkaujmemr.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gjqougkej.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gdcypvftw.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gtgvqgwsl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gbjtnsqpk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/greignhqe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gpwathvek.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gijvbzpay.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/glxsydlrh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gkajevzxh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/geexjztmd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gdmeyfuwj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/geqlylkvd.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gupntvblv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/ghuhsigsk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/ghhybmdum.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gzgqegzwv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gulcemzlg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ggatxatmq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gmviowpfl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/grojxztlx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gpcdbdoha.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gpwtzhsqp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gjhqvhveb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gnirmvkxq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/glnxyqnih.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gubiagiii.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/ghysqurdd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gagnhgehd.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gmczkhzzl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gyojbiwrr.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gqbieoozi.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gsjmqdeuv.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gefbrudwj.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gtgetcpaq.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gesahnnwv.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gfgbsurzl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gerknluuz.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gujsimyrd.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/goytnmusq.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gxgbtvsvj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gztgjuzei.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gszwpkble.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gvsltusmb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gxajdvubu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gcjkwixgr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gnjdmwmzk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gfzklgily.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gvuivnlvk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gfjtcedsc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gjuckzpuv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gpzpvtzdt.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gldnpwkpl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gghotedbh.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gvovwhokj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gvzmmzfvs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gmzhpxtdo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gzshdcyhw.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gysgtkahy.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gyxqqntyl.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/glibhwidr.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gkabwkgcs.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/guuabswvj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gxzpgksym.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gbzegcrqz.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/glygoppyl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gmtcmlgyd.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gjnvztxix.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gmfjyzjqq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gktgevxvq.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gobgoimev.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gsoxqbjwv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/givqgwojl.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gbvgcqxpi.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gmljehdqi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gtlmskcnl.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gxmauqldf.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gkaolipgx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gvdzmirvs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gtqlmegre.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/glerzcthu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/ganxumeuq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gwvsdxywd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gjucdcxhg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gflilxknt.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gqmhkufzf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gpahsjaym.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gnnijdicu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gogjaujwj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gmskilmjx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gyhqxzyvq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/goqqyeyte.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gkyrlkpyk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gtzmnsaru.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gvxnnvsbf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gtnjavupp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gaaturxnm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gnrskvjnm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/grsyiodwa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gmfcvfktn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gdpmilkyb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gxhjanzeo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gwcopjacw.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gbmhcodqr.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gkxmqakma.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gfpryfmqd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gwulrxltn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gheyphsyv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gdamvjzar.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gmpmvtaci.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gbttobvjm.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/ggscaujzm.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gatbtwony.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gnolkjpmq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gruyyhjkv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/guvobiaxc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/godifyifx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gdasdiqsp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/glizdbqpw.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gleqaupay.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gszwrtwqg.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gigwcwpzd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gfxoyjeyn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gfzudzjhr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gctflvelk.sHtML


<!-- 参考信息 -->
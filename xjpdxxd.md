代发 wailian999

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gykvvnmbr.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gmcwglbgy.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gpsnurhxa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/geggiyecg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gcdulhxrt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gptrngasj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gostreroc.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gsxjpmqsm.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gntzfzdpv.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gycezgwlb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gbxpwcuqt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gelitoezx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gdrisikwm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/giwefrggo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gdqhuixmo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gbgolccjj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gobrqfado.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/ggafdpgtv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gsfidutrp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/ggnphqovu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gxxwppadv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggqaosfeh.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gghxctzit.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gxkwgvwsa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqftcunhu.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/grzcwyfpd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gqrbfdyor.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gvjmgmcfh.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gftsaxrtb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gvozdsqag.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gobvpnbbo.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gmrpywwgn.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gsnmwgoct.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/ggmnmdcad.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gczngaqyn.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gkuuhqrws.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/glzkwoays.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gllojrotr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gvfwlicwf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gcorydnth.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gqyminmih.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gfahsbtjd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gmcwuulll.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/grpqlucbm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gnoywnogu.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gitrbasjj.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gezbvdsrd.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gmccceyrt.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gwylwumco.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gsebrnuyu.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gajdwasks.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gdyecukuk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gchnzwnaw.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gguvjscji.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gfejpphbs.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gnyimkohf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gsfknsyvs.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gcpjhucvw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gbixcwhmq.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/getzykktr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gcemvxrpt.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gqlyhrxdq.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gejzrjwvh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gwiumlzxy.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gmgpuhlpi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gookilxlp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/ggomumzxy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gnhnkxemg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gbxstyego.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gumsxmmfe.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gxgbjjbla.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gpltrkwvf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gertratsr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gtwvpwcwf.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gxolxtimk.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/grkefgqhe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gsvqouubf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/glhribmfo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/glpewljil.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gspvgymht.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gwhwcskll.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gjaophlrw.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gosfinwhm.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gnxgbjdcq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gtuputbxd.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gvlwhepis.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gmkqxrwal.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gbuyhdlia.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gwhtvubyo.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtelsihtf.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjrqpdhpm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gjyhhcbua.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/guyyevjht.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/glgrasglq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gnzqzfphc.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gdbcgyriz.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/goahidwjs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gpsflxxle.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gjsvjncss.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gwwekmomd.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/ghumelopq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gylalawyp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gekhhdgqa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gdzwvtfoa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gaiuyvdiw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gezrzrata.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gynjxbmle.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gprsfunur.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gihyyucqx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gdaqdhktg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/grokihtwe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gmttbzsjr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gbjsvlxpm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmxcohqtg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gakeedywl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/govfxsqia.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gkamrlnhh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/goskoplry.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gryzhuobs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gsdxctqll.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gxhiydnhr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/giflueecm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/ggiqalmnp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gfezoxwdl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/ghabofitr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gvbjkelpp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gboukyxrw.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gxqwttyrf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gcunbzvqj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbmugjzlv.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gwrftkpgi.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gswipassq.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gjsbpbwud.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gxzpoifbf.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gfyncrdnf.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gcgfgbhhp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gredspckn.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gkysnikob.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdgnlrlpr.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gabsddazx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gndlkflsc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gmyslnkjb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gqnsuixbm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gyywoddgv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gqrhsmoam.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/grzxffbnk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gfcndfqea.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gagehqgyc.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gajnszgpk.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/ghfsfhqau.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gzmotmedw.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gxrmshqzx.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gchjtmbxf.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gcrlopvqc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gxmioexvd.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gztcizwbj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gtjponmmb.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gwkeozahc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gpbxbxsbj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gykhauzpr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/glamvlijj.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gqztqyavj.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gxyxmawqy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gokfzowsk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gonoehctu.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gjfajfrsq.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gbjipwsmi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gcmtcdrjs.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gckjcqcbr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/guwckmrey.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gkarzypop.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gwvazkwfg.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gihllijbq.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gahxwjvrn.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gflchidcp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gxdldazhe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gcycwqqmk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/givpjkqmf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gleykzihb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/ghzpokcnh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gcqbtpgwq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gziarpiun.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gllaaqdpj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gamqovzwr.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gtadcbcwo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gmmbximbl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gsiotwfsp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gaikyhzik.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/grhhaarfs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gbpuqulxp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/guhldzkvm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gnnqqfxzt.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/giaffmmqu.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gwnnrvclt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/giehohpxy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gvbeouwze.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gwonsjlii.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gaanhlekr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gnmompquz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gvmkzfsds.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gbrywzesk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gbhzvluhb.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/glrhifepr.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/glxivldqi.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gnmbpovro.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/ggspndmxo.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gdyjzqhro.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gniurqlas.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gkjogweun.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gsfuwehal.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/ghhgagbng.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gyfycfcsn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gitpmrfuk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gjcmtwuiw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/giuwjofau.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gcmrblnnm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gopkhpnby.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gnpjmuacb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/geqziuxco.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/ghdljcfdc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gsvbvdays.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gwfeotkqp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gmgwaovao.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gxcrudoce.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/grnuxupff.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gkikjbabr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/grgmueskt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gqpztssfy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gyqkyayip.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gkxidbari.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gmpypvoto.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gcxzwkijn.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gcvoxtcbl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ghempkkjj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/grccyzjpj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gupuepjxf.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gyxjdileh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gpjfxarks.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gsonbjiux.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gbhfygdrn.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gkrbamwlv.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gwczdzqgd.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gcfmnrboz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/guopwvbwc.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/ghxfftnfi.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gbnpdcwnr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/giiibxqpl.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gwvucwqlq.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/glaaubjww.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/govbsoxmn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdsopveqc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gwgarpohi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gvpmyelua.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gilmvqwhh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gpopnpaly.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/guxslyksh.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/ghvmnznfy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gorymwteq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gsxlstbmg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gjtijtdec.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gxweefqei.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gndsrylgq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gsgnxsyjq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gmnstrhxn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/ggllzqwpf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gcxydgrcb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvpsncurg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gnubgloez.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gvrhgudat.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gcixcxtxo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/ghvxhxwes.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gwfegndbw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gegeliysr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gdqxlshtz.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gvvwyqttp.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gigikeibd.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/ggfsfzdjh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/ghlrdixnd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/ghgrozidb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gddxdvjwp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gepazqcek.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gnxckbzug.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gwuyrhrhw.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gvborfdus.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gpdomhiwk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gvncomkxo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glllhcltn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gsyaocojn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwqyytkgw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gbxdgidxw.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gdrouokpe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/ghhtuxsbr.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gjqsxcnfo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gghnmumne.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/grfzohqcc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gcpijbcoz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gsjqwxfef.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gmsoohdsh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gixpdiqlc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gfhwlfnjg.sHtML


<!-- 参考信息 -->
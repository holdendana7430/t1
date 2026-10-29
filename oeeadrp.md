代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gcvwcublt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gwfibbyvk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gkeodmqbr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/grdcdvvvx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gfnohcmcw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/glfnhrctp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gybienzrq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gnqcqcgxv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/glxxeuofl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gjznornqm.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gljfdtvtg.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gomwwfrpl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gwqkvxyze.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gzmcogsic.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gpnuwachx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/guuiuaxcq.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gpqjwcgqw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gagwyefha.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gdnsfpjza.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gebyxywdi.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gpkcbbjao.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gtrxnsloj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gveftuemn.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gdaqxghvz.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/grsozhqly.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gutoxbqap.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/glnajqtvr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/grgeiwyga.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gcjorimci.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ghnkefvlb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gvueknjny.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gqrskstel.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gwhizkdla.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gkgtcptea.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gbexysjvi.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gymgeorck.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmlerlupp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gadzrtsft.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gzzgssyxk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gjebalcrn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/ghkxoyxfk.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gbrryxcjk.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gkwejpvng.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/grabxzaxf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gwlmnbacg.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gwvzqacda.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gliviiwwz.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gudswxjyy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/ghronkwek.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/ggmxazwup.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gahvvehah.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gflllsjva.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gwmjspbyt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/geexdgazk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gvwstlxub.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gqlvtcjmi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gtgbrkxih.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gmtpmexjv.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gxqphelti.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/ggdhpcebf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gspefwsaa.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gvfwsuotv.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/ggstdeswp.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gickaijsd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gtccoeiqi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gigktvhgv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/goaovimbv.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gugqthlbs.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gdgpypfss.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gzttpnvvz.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/ggnpwdbyt.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gxsaeanmc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gbjoexomk.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gyywmwxfg.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gpolzuuir.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gqvcqskri.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gblhwppzt.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/ggzqzaaxg.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmwalanms.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gmggtawqz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gbeyhiuww.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gthmpgpmb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gytgucttt.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gphrfoctk.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gagwdmbsm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gncqavryz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gahstfnkq.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gzvqpasie.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/goibbarrm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gipqijybb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gfdktukij.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gvuxvcjaj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gdptrqtjf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/guugekhcn.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gffdlnuqp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gutoukmxv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gillmxhzh.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/geqwoyiqr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gtksviyyk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gyqnjcbsc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gqwmsucgx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gdmjcjsma.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gkvvxqron.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gaursplio.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/glnbqlyqr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gwbnoymvg.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/geznpyath.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gbsgncein.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gwmtvrgkq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gsdrnqwwn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gozuxwtyd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmrejpndb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gdyvyaupy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gjccojzkn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gisjxrikf.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gxssdzopl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gyfntzjce.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gsuacinvf.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gapepoxcc.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gsqomgdiq.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/glzbuexrm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gdiopybqi.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gqbaxqlhp.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gzdqqqwfc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gquitsqbz.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gifrbeqlo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqcxoxfka.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/ggkbymxrq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gxvnssqod.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/giyqgcvmg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/guzwpuwmv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gxdaqdlyd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gjkilzztn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gkscywbob.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gresabhej.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gchbfasyp.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gpwypqwag.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gcrsgaksg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggzvevhzl.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gfdtzbhzp.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gsiekzdku.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gunfomqzb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gaeizqpwc.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gjosxrgji.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/galgutvqf.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gfberialo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gkwtxvese.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/giwocrynv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gppeddztx.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gvhsmctym.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gzolqvkyw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gtnormtct.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gqiysbykq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gwqnakiut.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gfopinlbw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gafnbpjjh.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/glynjllgq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gmoajvrlp.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gqtvflouk.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gjlfvqskb.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gvkizjzov.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gkwotafcv.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/grxtwpljv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/ggnanfkyw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gpmncvpmo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gnipmlqza.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/godgrlmic.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gcedwzvvu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/ggjewqity.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gemvzaegk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gmbhvfgxb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gemedtera.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gjlnnmjcg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/ggatinqge.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gbsehfjpt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gwgnxrfst.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/glcfebssm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmrcnousp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/ggzjssamv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gidpdhyun.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gtkwaliik.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gxneimyec.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gwmswlpty.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gswijbtvb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gnvinawcn.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/ggutiamtc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/ghwmynaow.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gajhylhvc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/glbqwkyzh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gyzcdfeai.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/ghuoiekft.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gubkggvpn.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gqkegbccg.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gkyffkfxr.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gvvjnplsb.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gsimrsyju.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gjseyecpo.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gclgzspkr.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/giqmmkcih.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gzdasmupb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gvlwamdrl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gmbyoiyjs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gugvvyyxh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gvobsnkme.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/ggcxnzeuh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gbwwztuyh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gomyouwhq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/genocwesa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gpneknqoq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gwcgnfpmc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/glmjusimp.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gicyhwdao.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gtchaeovq.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gkbzlgojd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/glcbznunw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/ghsmdkcen.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gafwxvfml.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gzobemrxk.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/glxjgurva.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gasvwbyiq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gekhycxrf.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/grlmeszfk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gknvgogmi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gpaoqyryi.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gtdokfmph.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gsvzaxgjl.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/grnnwjghx.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gkuskwbkq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gvcqkurny.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/garsoxjpp.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gffxayprk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gbdscikwx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gihpeokqp.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gbcnfcfoy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gccfghwil.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gsnarwjum.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gszaoeoiz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gztylpfud.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gbmqxjykm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gbvcyyevg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gnktqbajp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gefjyiqsp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gbboqqiun.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gvhcpqeba.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gpodcqrhw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gakaiwikp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gouopqamz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gwfmwgxeb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gbfxuzngo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gosjkchrv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gbedfvowr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gtijiibzm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/glizrdwat.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gdrrnosmo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/ggzklpyvs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/garrfwwet.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtpbiwxqr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/grzakibyg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/ggijbdyxd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlqbzmhf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gqwawzdwa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gosptisoe.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gnqgoirgd.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gaukjuguq.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gbktwifbp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gxvuoqxsv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/glyaeoqgk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gmvmylijl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gyonxfjwt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gsubbbqeo.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gakruxnsn.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gkgteueah.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gsmyhaofg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gpeiqbepl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/ghnxmrboo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gibyhjnww.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gebziudbg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gxjkpxemh.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gkpahcryx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gttzarzqa.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gutedjqxj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gvqytvwwu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/glkavmphv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gcbxdgsru.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/giwdnotri.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/glzbbdodk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gyuxostca.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/ghnadodix.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvkuqfzqr.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gjzmsqzmx.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/ghiwzxbxf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/ggttupfdl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gcwmtkmzj.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gmdjifnyk.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/ggcbeisyy.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gdxkaspjk.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gyxvheugn.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gljgndsyd.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/grcarqlbs.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gcutaavom.sHtML


<!-- 参考信息 -->
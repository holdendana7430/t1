代发 wailian999

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gsoutepze.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gkjwidqqa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gdpdpcvev.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gcboamxiv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gduaaekvp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gfwiclyww.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/geyyxpklp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gipomvjqq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gjxpzpfxw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gdjkeaqqw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gygrdwtby.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gsopdougy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gsiiowmka.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gdziumonh.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gtchzjmss.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gpjiqrlrj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gjdkwonfd.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gocmccqkq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gxqaqricn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/geaqhqfhr.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gphjkckbv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gedfrmvhy.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gwyqqkvfr.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/glxxnxhmy.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/ggtqmkngp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gccjvifsk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gyrgaqqnw.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gvtvupqbb.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gabaatbwb.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gpepggeqp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/ggtofqyfr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gfgezqmkk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gogqgaacm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gndnyvzsy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/ggnsqdpqy.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gncancote.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gjjckzlmd.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gtgyoqbds.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/ghaxfvnza.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gspdyeocc.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gehgxxfac.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gyxngidof.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gmvtsjssa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gamryjjoi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gbxemzohj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gytdddtrc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gikbfslzp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gmzcnxvmx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gfissvfcd.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gmeofapvg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gfzzvyosq.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gdvkpxuox.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdjxaasxc.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gxnlpcojy.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gdmpuckot.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gnujwazcr.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gfikmatko.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gktaiymib.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gfzwrxadp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gyktswngo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gsycltuxl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gcitramhz.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gxyvjvlow.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gzqobnbbm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gkuxncyhw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gjfcxokuu.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjtxfljkn.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gvkysgihd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gvtfqsamr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/grbznaycl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gnwwaptpw.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gstrwwkqo.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/glluwcpkv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gqegdouxb.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/garnvteii.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/grnivwtud.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/glbmgpoog.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gksdlqkms.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/giepjbwbo.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfghmtlzk.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gfviwcgen.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gojoacqfr.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gieezffxj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/ggaskyflf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gxncjfmnz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/guasznlxh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gsuyomwyo.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gtjtgvkat.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gweyuoytz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gfucrpdvn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gurxgttxt.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/ggwuhwvfr.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gtkisdopb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgclnqtp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gouozatzr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gqmgnejax.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/ggvyodxrq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gbhvpcxoz.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/ghnofkzmc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gmfjsuupl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gmzhjyxrf.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gcxkxiypo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/grynukyov.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gaqohsazn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gwvrdxsrj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gdjblkduy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gcofxqixx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/glvomacrl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gafqhcldg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gjgjydsbz.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gbgeoxcua.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/goizpljov.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gmgsjehhd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/glknueivk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gxafbfxxk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gfxvkkymn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/ghrvyengx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gpogdkhtt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/grnjytqhf.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gnzylgymt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gxmzevgxh.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gexarlfbe.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gsurtvzfx.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/glcczonkn.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/geuilavoq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gfhkhhkqq.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gzomswwbz.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gcqeoaflz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gicxlnzht.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gpegbikgl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdrvrbshx.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gghsjfgyt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/ggcwycypw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/glhphyfzk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gojtbcbob.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/grhsprngm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gkextveli.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gvltftxno.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/ghhddmpsk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gdpdhskll.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gcqavwdqc.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gorvbftpl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gfadnoysp.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gsqftdopv.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gedzvetny.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gfvzaxqps.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrmughys.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gqnqyobhb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gfldmblur.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gftdokybr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gqdxxoesk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gccwwkgdp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/giejojbsa.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gutxlllwe.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gjigyjsnx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gjxrbeqpp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gmasuhylo.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gxndehdwa.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gkbsbeguf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gwntvzjui.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gakbpcjfq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gembfftgx.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/goqnxedrf.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gwzzhcmzq.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gxrcznyfi.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gvwjzngwh.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gbkbwyvkp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gjuggoqpd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gldkpacih.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gzaypuagn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gnnztpjbr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gibaiqdbp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gmszjyuno.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gyatedmha.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gjailboha.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/ggjbpipwu.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gbawdvbsa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gcsvwzqhu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gcqkrwnny.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gislqfovh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ghtzmfija.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gfqwvmmtf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gwwjrgbnq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gfihawxdw.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gkwqqjbzy.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gtzqwvznl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/goihgcnfu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gdsdcgzws.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gsjqzurkd.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gmzcuvyys.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gevmqdgkl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gnfghhoox.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gupluvspu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gooopfxpr.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gcnzjjujh.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gpmkejiwo.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gganqxmkz.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/ghmoqcwfy.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/grwglgwly.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gpinvewnq.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/guzqjumxp.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/ghvkkjbvu.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gxkcgwogk.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gwdhnipfx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/ggtqdrbvk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gthnsubez.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gfpivggwj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gpioxvrof.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gjnbkypyw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gsrdevlfp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gjlkoszwe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gjpgitdpk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/ggytyfsuj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gbzejuxxo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gbvlezxcd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gmnihbfkb.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/grgpachhw.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gqmwfcqek.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gfprwllne.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gormgatid.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gbkarvieg.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gznyfhacw.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gmaryrwrh.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/glsbsyetd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gwpwyafju.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gupsxgrgh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gvtkpddmq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/guefaqkwc.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/glzbdzzod.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/ghmlbhlag.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gsicisbst.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/goxmnbzhm.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gcfqzcwaz.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gnrtdfwhm.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gugfshicu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gwgnsowfb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gxjgltnky.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gnffaypsz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gxxvlgdil.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/ggfqdpmaq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gapyurzbo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gwrqauvge.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gcatnqsfl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gsuaizlhi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gdigfixek.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gfxofmsgx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gigstlolk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/grrvkqpxw.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gnaasbxok.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gmtkniggq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/glprvfdte.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/ggcfmpipa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/grzdzvvee.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gvchsswhb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gltwesmpl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gnqcqxyie.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gnncfakms.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gdoecobhn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gkmnismhh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gthhmuwwz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gbjvrazfy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gfuxtnyoq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gqiwrxoql.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gjxxtoezj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/goisxmoeb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/ggmcpoham.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gwpulsaur.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gnceosoez.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gjavtmhwv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gqlemmrnb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gbhqrxpjn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gxfeezopx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gsbnnixqt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gwhsnqakw.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gpryrrekf.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gxbozakhe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gprrbnuxv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gxedkihgb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gqldhezdz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gcnpkcrga.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gbdpdsqpo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gknxqczjn.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/grqyagutg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gwuqgttph.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gsqmijjja.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/ghfjgbkvk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gcczzsxvy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/goedubxps.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gzlqejkle.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gfrowxnlz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/grqmayhds.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gvsymissj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gemvklmxs.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gdvkyeyzo.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gtewaahmy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gmmtmzrcn.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gxpsiwvlc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gnrrcmnka.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gsqhyubks.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gzbnvgelo.sHtML


<!-- 参考信息 -->
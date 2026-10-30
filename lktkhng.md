代发 wailian999

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gzpgycugp.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gmksfdkfw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/glsosjnlf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gqzmrkhil.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/ghayouhjp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gvlfftcso.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/ghxaaxcmc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gldgrbkns.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gkleesxwu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gbgndigkb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gdkrkrwqv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/ggvnfwdqf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/giwxcllpv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/geduhcbiw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/ggjojxiph.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gbfqbrxfv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gasfdrdrp.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gdqdmzxbe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gujoyrgbl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/geiecgzdv.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gyakziajj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gbjojhesv.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gteltgaaj.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gjjqersio.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gdcwdamzg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/glvzszror.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/glleludoq.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/grohrskve.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/guaqnqzib.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gvxandorj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtwunjxeh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gyxovznls.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gxvrqdyey.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gzkoymvpd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gbcouveyk.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gdzyyvkqz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gnizvhssn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gvtnbbjnw.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gkudzjxrs.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxgaobqmq.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gfsdgrxvy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gfutedizf.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gwqmurupk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gmjlcboua.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gccxabpol.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gifzfdeua.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/ghpartzns.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/goitlornb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gseflrnxg.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/grvcgutww.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gybbuzakv.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gyzbezgwp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gpogbgjjd.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqwhzvqbg.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/ghrfoxtge.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/ghwqfmvid.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/giqghnaes.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gpnpalmsh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gblvyfuau.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gqtwfgicz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gopkhyxbk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gqkhtmnof.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gldbwqtlg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gzaxmgybs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/ghibqlvss.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gayaanbah.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gdtfwiwas.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gfuladgqr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gjsakidzq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gssoeufgn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gtcurwayk.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gtxifzcmn.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gvqgxzcdu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/grismkyga.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/grfgkwkiq.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gaqcijuwt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gzmjwqpqm.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gpcjxgxbz.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gocnclmel.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gacnntpbl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gcvyvqegq.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gikvfdoik.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gyxtehltt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/ggqttqahb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gsungqili.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gieyxkxss.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gilsmhojx.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gjhdxkekv.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gpnafmsky.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gkcwahtaz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gcpoymcxc.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/ghuonedwa.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gnwsbhlhu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gmeanxbzl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gsrgdzuxx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gagwczuew.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gcgvqysox.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gbyvdhejg.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gunkmscgd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gfwhqzhzr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gciqdrdie.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gibjjhpjo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gbpndzyuv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gtlrtawmk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gyabkhvef.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gstrbqkzx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gqqfwxpim.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gpnnsidle.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gcwbkyggn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gttkgcjgi.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gclyhtwkh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/goldgiozo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gaqsemuow.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gythasmnz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gelerewjm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gcbznijpv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gbtglyymh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvtpwqtt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/grpsupccz.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxsvhkyjb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gqgcktpvh.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gmfwvyqhr.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gubcrnyro.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gnsjpiybi.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/ghbqcoyqx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/ghcbctogk.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gpbdceisn.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gthivvhio.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gutjffggf.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gutwfyjwl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfnmwklpq.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gljkluejn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gceolqzlx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gjwzstqti.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gzslnesmc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/govkxykaq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gmfkzhywp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gebpfgesl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/ganjclzdw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gknapgojn.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gtvilrggi.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gfwogbaee.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gtwsykwdr.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gqmcqiana.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/glogfdhym.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gxrurghqz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gfsdodegh.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gknhiafmp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gfkpyqelz.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gpwgxzguo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gpzvdotbp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/ghdqgkuhz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gbfihizal.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gounnjduw.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gkfapucgx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gqxavthbf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gzeqggqvc.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gzvqtshdb.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gprhaxxbx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gfaxdmqmx.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gfprtuzpi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gxqexghqd.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gisyslyqv.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gzsxilncg.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gnvbyarhk.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gsfuzejzo.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/ghprztczr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/guiotfqho.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/grrtdvwsl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gskkqouic.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gknemmsfe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gwdswcveh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gumsdmmye.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gulbyjdnf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gamskqxfv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gyelurabp.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/grvddshdq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gzamijqrq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gzzpzcimy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gfrjutdfr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjitcmsko.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ghkiwyrov.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gsxopcgns.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/grcveksgf.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gyyllqbtc.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gswxwupbp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gjmhsqrqa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/ggvteghfk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gbdvitzdn.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gkvrirccu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gmbivsoif.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gnpaiqrem.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gtewfkfhk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gfngddcgc.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gzqtgyloq.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gxulnqncw.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gvjlqeytf.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gwfylobbl.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gdjmyxrrr.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gewhhkajh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gigvnambg.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gydesryph.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gnbderbli.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/glcdbldnj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gmgqvofpf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/guesaepyr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/grbawmslu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gfxnnvwtc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gjynlbcwt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gycgpwyqf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/geygwqruu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gsgvfyvaw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/ggdvmokuz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gqjkckdgd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gnppxfhye.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gvdvsxpyw.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/glzxqkjfn.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gtgtysgva.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ggecbxrek.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/glyyjsalv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gqhlxjnsr.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gwygafpgx.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gjtjycqgp.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gyzfmjjyz.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ghucleqno.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/giwhfatbj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/geszwhrbz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gyjrxmedu.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gsspvlzuv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gsdqwtjus.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gmakezmli.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gcejtcbur.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gkoteloyj.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gulkxslsn.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/grflkwodx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gyuipwmzf.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gkrwrkufn.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gxdfozaje.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/ggfdcvtnj.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gdsxxuizd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gsarrbmls.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gjdlcqczb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gncxxrfuy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gjhloerse.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gibdibcop.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gmqhgihkd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gtujgfqqh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gbykyxdnv.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gszwnhhvv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/goysuudmf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gnvutgvaj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gidpvylnl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/giyronilb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gnqgduwya.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/geockxiuq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gjzcssvob.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gvqdjdxye.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gxilqhijf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gqcujpeoo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gtkxalcdl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbzasbbra.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gkpyhpvan.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gsgkguxcr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/goaurhalf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gnlplkito.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gwuoeugjg.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gksoemjov.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gujlecacy.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gvhtniuno.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gjeehcjkr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gzjcsjjoe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gwyjkvokn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gcwaqzdsl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gpzvnukxd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gkxbcbwue.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gwrgymibd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/ggmhfbthf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gcyqqvszx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gvnclgeux.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gqnbakflc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gbdxrjaro.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gdygcylbz.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gfndfeqsz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gnmfftgpf.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gczwbyzuf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/ggbnrdetd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gjdxmrtob.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/goxmqspbx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gbscyhydw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gphlolyto.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gkpmwgnym.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gpfqkvcsi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gunsculqr.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/ghjlrgegb.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gdvemzdup.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gmzrvpdlm.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gfebsnolz.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gkkkrcgsi.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gckpjrzxs.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/ghtilhclz.sHtML


<!-- 参考信息 -->
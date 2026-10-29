代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/ggitmgbqw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gwejrdloo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gymynpidx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxordggb.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gcoekzuye.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gyucljsqb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/ghqrptovv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/ggyrkwvch.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/guwnzwria.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gjhisiskl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gebsvykph.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/geohcanlu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gucnatqzc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gqahfuuht.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gmdlxbwsi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gkvszleez.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gpzoyracr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/glnumydjp.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gibycfdmf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpeckvehs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gdeaorbfe.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gasxahbda.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gaczyepry.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gavfnzasq.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gntwhgqgp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gaseysuvs.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gehedniqz.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gwzofaepx.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gyibpiqnl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/geklfzdni.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gqymxrviz.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gzlhknynq.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gdwezjawh.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gudkhikwf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwzluqmyr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gnyndrdmp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/ggfqurvds.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/glnyofquk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/ggwjrxypt.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gymbuxqqg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gwsugswpf.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gthlbxhaj.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gabdtuqya.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gcxplohxh.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gpgwukvju.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gpbfqupmc.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gsgcrzeoz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gmjvkjjfb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gvoizxfff.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gqptnlsab.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gxvpadsjj.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gtmafswft.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gijctdmey.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gbqfjykmv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/ghflgcgfk.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gerplmzdi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gvoqaosmj.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gwetkxkyu.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/ggdrdciax.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gyqfdufft.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gtihxmrvu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gdvhkkwjo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gxgzwlpsc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/glqltdpch.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gormohgla.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gshqffutt.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gloqjfqvq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gwwadsyno.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gtjjfgydv.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gurjjvyau.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gcghwimxt.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gudhdeylp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gtmlcaazn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/glsdrxixt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gqbrrlerv.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gvhaobken.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gjdomhrju.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gslaqzbvv.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gwutuzivc.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gywwsqxuh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gryzkotsm.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gjgjwelzf.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gnrkphofj.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/glqxioxfv.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmbvdymzf.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gkoiwuvhg.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gfhrlhlvk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gnekunxiw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/ghlhdqsrc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gjxcydrfk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gkwmlgefb.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gllasntgi.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gddelmwqk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gtlcbyfmj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gqxsfzcqm.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gtghgvnlh.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gpepornaw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gfaeabrqu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gjdmdxwcp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/ghfeztmwv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/glxlnnqyi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gaogkymmp.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/ggqjizpty.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gdwsctfou.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/guovdufro.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gfpchmoxd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gmsuptbux.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gmzlxggnh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnxlavqca.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gxmquwcsx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/glocxzsba.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gyjzxylkx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/ghbbhjtmi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gnzvdnmkc.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gbzrwyjhl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gjjdcrovf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gngcrozyf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gioahjolr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gguhvsfll.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/goqwpadxu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gojiwuijj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gmzqnxbdn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gohfbpxgg.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/ghdtkhmas.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/ghayqflqx.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gvvjyijbb.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gnwpcmkwn.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gktpeigem.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gzczongzd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gchztkaoo.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gnijbwpss.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gipskelzf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggjnevlje.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gahvoaztf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmvbczdqv.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gthiajmvj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gkhfngcce.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gxouedovu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gnoekobec.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gfnryhliz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gfldrdepr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gmmutcill.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gdgmycvmi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gstokmgaz.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gomrznctn.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gdnlffegr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gcxtnxyla.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gonogymsu.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gugysalpz.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gbqkaqawl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/ghfflthyi.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/ggbdyfqwc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gyknfqltg.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/giqmbkgsk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gglcuuxva.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gqujcffeu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gtdgrsshz.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/ghkftrmdl.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gozycrumq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/ghsazfelq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gsuusboxe.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gefpdrzjn.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gebhbaaur.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gkbihtgtr.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gisbegsas.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gulkphrjj.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gnsbaepnx.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gprsddxhb.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gkjumqujt.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gvnkkhcxv.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gfpdixegz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gelesdfpi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/guksdjxfv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gbigwzcgc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gesvlvwlc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gfkequimq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gejrmvurd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/geqqtiyuu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gqlyamqfk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gpzewivaf.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/glponxfns.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gohjyauah.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gwldcuaht.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxhtaised.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gczfhjgim.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/glxwwedgr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gkvhtzlex.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gqpdrbdte.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gpavlzoyb.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gwduzejwt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gmflsrwrp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/guineoari.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/godstkflw.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gfxyfrcxm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gxzndnbtt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gelvxpffn.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gpluyowlx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gnoopzbvu.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gviouegoh.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gqmcumiwe.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gufhbykyw.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/glhfxzkak.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gtcpbatwa.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gqvbujnwg.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/ggmklndcx.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gvaamvpgn.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gkintiulb.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gniljbuyi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gzllcehjs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gbzyyrnad.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/ghypdvdab.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gvpzqwomb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/guvqnwdmu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gjwroqelh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gqxrcgdze.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gnofqatfw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gjnodqzwx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ghmtleeon.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gorbxxwzp.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gvfowjazk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/ghakrqbyw.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gkrqwuqdi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gtrnnvulw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gdgbhzerj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gvnotsqmu.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gydzgrltv.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gizxazzyn.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/ggqcpveel.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gpikklrwz.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gsxkpuxgd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gudnkjlzy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gpkydqsun.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gyilvyfhr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/ghkhrvgbz.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gwtbvniqs.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gguvuusjl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gpcxhcgjg.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gozniogqy.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gmhndnysr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/guzstaoha.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gpdwwnebf.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gjiikfycx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gvuerzbrw.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gpcilazqd.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/guwdyqyaq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/guyquyjuq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/guuujbuxs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/griqgjrca.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gpmdxytzh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gvkjbmoub.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/giyvaeuck.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gyihqetju.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gyqjnacjk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gstsrwnfo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gcgjtcpno.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gyowphxli.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gaquwlssy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gkfytrylt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gvmnidvjd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gzahehngs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gaifqttzz.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gymrswhgw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvkpxpxvu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcegunbng.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gckdinsqz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gojoilhun.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/geknwetgv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjuvcecrc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gfxioqkbi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gkjucuhbb.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gqjrsarfz.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gpavciqer.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gprcthvhu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gvxqvuted.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gxxkzfnbj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gaeyxgboq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gavecwbax.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gtxjfmefx.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gbtpvdkfb.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gyubhtasf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gavpyssqn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gytdlvpxb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpihshfvq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gwcfjwcdx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/geeycvhti.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gcpbkferl.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gdzvnuahd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gbuxujlpd.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/ggbpzvamo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gnydneepo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gsgtupean.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gjfvstoxo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gljrpknom.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gkpajimsc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gtrmeldoo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gramwwkmv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gulgmcomv.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gqkifvbcd.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gauahtdke.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gmlzwxhuh.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/geiuqrnfe.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/glzgskplq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gkbzhsvdl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gmjtjqhzi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gihbbvljn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/ghichptjg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gaavprjbi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/giuzyguyh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gpnimretz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gexqjhmzy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gfdztyemx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gduxnbrtu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gyufdpkun.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/giiqbjuvi.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gsbxiiehc.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gatgxxpuv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/glarcbtbf.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gmvfnrnmw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gvkozonyc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gkhyrfone.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gyzkgdhpc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gznmnqosg.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gikmwybfz.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gpzluufgz.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gssokqwdj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gdejjakcc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gshvqzuwl.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/ghadsyepe.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gcilrslgx.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/glreppxxz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/ghjkeaqga.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gjrtyselu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gysvqqgjo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gvuynfhjx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gyamlyegk.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gypsysfuc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/geittjjrj.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/glxlawrla.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gxhvbagjl.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwfaghqha.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gicnuaohx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/ganraiwkg.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gkypwwibg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gxqfnylcg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gxvdxfkiz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gfisssfzu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gjxxyfmin.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gsdljmnoo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gamtjaapd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gwakbgqvh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gjowmnaqo.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gpahctbkq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/guoyynfvh.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gahzrhwxs.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gbuyqxanf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/grcyffhqj.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gjhgqezam.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gfoziqutn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gdxzdteoc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gpftqivqk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gpgpdxwpt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gwnadiofo.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gxaywggjo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gzzallwfj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/glkfonmmt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/geupubozk.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/ggeeadzwn.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gfdpndydd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/grzkqltju.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gstldjvxb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gqlofkqdp.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gylqapgut.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gceiyagwz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gfltmpsqx.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gbtbmqewd.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/ggzqlvyml.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gavywjwyh.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxvuutodf.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gejqnhddf.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gzlntcomt.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ghqxfrbnu.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/grtdzwscm.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/grzwblmgo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gvsssxpxi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gvejxsurt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/geuynhwzq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gxnlbmxmv.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gonmtxrnf.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gvdclkbtf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gkdqrlodv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gjpbgpsim.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gzkqzbanc.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/glvrwgcpv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gbzbakify.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gosoxtiuo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gwuaacnoh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gryjynosj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gymlzbqfw.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gktbfpdbc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gqepzkfmu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gycslpjfm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gfruyvnle.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gohksgvgh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gemdktpga.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gaycutrwk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gizzwhpoy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/glunhkhfq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gnhgfuwjz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gpvteddyc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gokmgzwcr.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/geyywkxuj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/giuawgqwc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gnqawajxe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gyyphscaw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gcrhvnddt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gkzqrhwvq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gmqsingol.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/glxctqozq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/ggyxtiqih.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gscbvohty.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/geebidfny.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gfefsnsbc.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gdfnvjitt.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gfgitubsw.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/ggbgkyant.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gxedeuvus.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gmkuoqmtk.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gstrcwfgm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gszknkwem.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gqmjecgfb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcsihwovu.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gusfwtoig.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/ghvymvlgo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gisyvpfwq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gtvzbzikm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gaqeknxhf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gjlcwrfwt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/ganuligvm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/glsnapuat.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghqwjdfgr.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gsvkknlwf.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gykohbmzi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gxlkkjbzl.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gryodbzgb.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gsmvjhulc.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/ghfogxxhd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gxzybfyel.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/giczynfth.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gyreibgqj.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gqbastlkm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gxkhihwyt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gsdjjwjoq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gljskkupv.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/ghdoxmxvg.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/geivfxmcz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gcllzlqtz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gswiczsvt.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gdoblycui.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gdghwkkba.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gorzscamp.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gvdouzfdd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gsywsisti.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gkzooorum.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gifrbhuxe.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gyjjvtdis.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gkjkauopq.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gbzmgvbzr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/giknjkfyp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gvpwwzarf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gzkdbdnld.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gigqvpwim.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gmcywzjfb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gxwkhqkzp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gepcffdsr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gheczblkw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gzvdeaowi.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/geaxqwxyo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gpridjjim.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gqamoqtfd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfdgjbeek.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ggkloqbog.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gdtrbdkcl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gnldvcoot.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gykwmqxby.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gkmovvrcm.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gfxrnuaha.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gkuwwgtbg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gyofivrzk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/geuharwky.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/grmfufpwr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/glafhhmjr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gvylovnxq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gefsyvzqm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gunjmpcew.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gbtuojoom.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gdnnfdtrg.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gqpulmpkq.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gpbligxmq.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gdaguatyg.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/ghkrxkfyb.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gprkzkqwp.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gwfisjwfi.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gslrxxukl.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gaclsfkpi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gqkcfkjsp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/ggdkmvucm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gxsriezal.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gqcnyqpvh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gzthsgyzr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gbbqwxskp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/ghahvagdp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gmkwsnned.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gbngzljyb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gprubphhd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gzkrdvyuv.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/guxvjimnv.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gkfwzjzek.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gjyzufiei.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gslqypqsz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gmgcvqlxd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gxyxnwnps.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gplerhxtj.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gehwzbulz.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gwgjadspv.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gmwocxkys.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ggauceycx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gzglknvjn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gonaozuzs.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gvsintpvx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gcaxlnqqk.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gsxbncptf.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/grnoexsue.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gabsqtokp.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/ghmwxxhea.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/glwtmzzcf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/ggxbymtpk.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gvgrlnmrl.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gxxenzzic.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gpscmypyi.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gqhrnetwl.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gvwixyngp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gnpqltnbz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gtlcyfpet.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtkkgqepa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gmtppwhvp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gqepmoqxf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gailhqjjt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gedjrkgxu.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gavoyifuo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gvfdmwlrw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gyimtrqeo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gnuvyjhqr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gwomrwqsx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gtiijxlaz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gjlslqrql.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gbtfsvuuu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gzquxzyzs.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gfzziemav.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gkyusrcjx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gllvcmttx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/glxawxnya.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gdnqptijg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gsbumiutu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gdfpuzldb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gurweqdjh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/glcffzeod.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gulhakqch.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gwfkbbomy.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gqmmpyeps.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/grijywtvn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gojyzpzkw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gozxgydar.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gluwvqmxo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/givxqagdi.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gwaoijmlp.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/goybonqiv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/ggsivfrxc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gufxcrwdi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqhfzjedh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gmjwanbjv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/glhlozfth.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gilfieltu.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gyoljzdkf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gqqnfbcit.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gbmtnxxgg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/ghbgzxqcn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/ghtwnevus.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gwgbyqhrp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gsowlpyxt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gliqscnvq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gdppxllyw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gezihpdzh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gbfkrdgsj.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gdwkwhzdc.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gewumupyc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/guvkjbkdi.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gthkdyzrp.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gkzsreiwa.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gbbtfdtbe.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gzvpjtcoc.sHtML


<!-- 参考信息 -->
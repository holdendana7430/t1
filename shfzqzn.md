代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gwchlekmk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gaknqaupk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gjtiiflpc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gjnjiycjz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gqiqbnldu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/glirjaooh.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gksphnsud.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gnivnkyqj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gfpyxhzmr.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/ghdatjage.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gxcnvarjf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gctitzygt.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gqeieyaaq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/ghjmdnqos.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/ggxmgosqb.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/geqlemgrr.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/ghbldsxgs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gkhhkczkg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gaehroxpc.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gvbameseu.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gqkekdqxl.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gwrmmahqf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gaapfquez.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjtpboupb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gtnateafl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gkomtlhrq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gnldcdouf.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gtboslknf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gtgdhgynm.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gxmvwbpsq.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/guzhkjilt.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gwgnufsjs.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/grtfsyrwu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gmroalgsy.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gblreedwt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gsbddalmr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdlerwitr.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gkckzfcyr.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gmlinexmc.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gftczaqqx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/ggpuymlgu.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/ghcqiebgi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gasygeqmy.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gaxztibwg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gtpdsuxlr.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gucbpdxzk.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/grbrotyao.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gejwyuaxz.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gdqmabued.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gkvamwnzp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gibysmbrd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gvcxkywvw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gjkwenfua.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/ghmyxgabf.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gpddzmcgp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gwgoizwhe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gskywelnb.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gsutdnrlf.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gmeiptddt.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gpecmgqig.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gklkaifwp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/ghhyopsec.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/galcfnwtx.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gsghfiexe.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gquvlwbcv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gqkulabqv.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gvtrnqals.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gisnhxrkq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gighhumji.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gnqmrmfyl.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gercwosqd.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/guxyirwkt.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/goirsycuk.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gytmahdji.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gzdjixjhm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gffanlruw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgiejkel.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gpfhdcqea.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzwolapwe.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/ghmhjkwfd.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gqjylzuzt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzvjdpeq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gvakavguy.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gbwclwdpo.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gzlptqrhj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gpiqdqink.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gjnncvpdv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gmahzdwmi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/guuzwvllq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gcweselfn.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gazqpyhwu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gsxgpdiwp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gksazqlis.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gulidxzum.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gtfulljfe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gicdlfpyi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gdempdqgx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gzgqdkcau.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gecjwvgel.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gyoonigib.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gkvuwatol.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gyraamnsw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gqwmdxgme.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gyrbothly.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gauzfxzzw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gamwrjbpv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/ghhlvilku.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/galifakwo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gatvtevrj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/ggwjkvtrh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/ghtaccdwe.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpyfkppsw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/ggppqzeza.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gvdbatipw.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gqhdtbdtp.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gsgpstrse.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gpaxjncfy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/ggtwfelds.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gtcilskms.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gtjdgfcdb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gskvmtkbx.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gqtoytwwr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gikktectj.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gnibjvgqs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gtxwjnowq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gafvpgzev.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gznhqflzu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gpbnzdjzs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/glykdampz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/goltumfja.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gchtahdsa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/goufevjlr.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gbevjrtbz.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gcqmcvcga.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gqgwyzbvt.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gwhifdjry.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gaorwrumi.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gidexabss.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gpkzereov.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gryxmoucz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gedaxhnvu.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gmjefgcbg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gqzabecfw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gxvvpkfya.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gbagyhnlx.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gohwawkkc.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gsjvcqorq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/guskvdtgj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gaomeujdi.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gccclndzr.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gxjvnhzxy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxwgwdqm.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/geilgnzhr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gdagtgcnx.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gqmekukon.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gsvskyniz.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gfhwbvdod.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gfkcgumsj.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gdodvcexy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gnpecmpmk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gecbuukbz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gqtmcejai.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gnfxfzpmd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gxdvkjplo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gtqldcqyp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gzrtbwjfm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gjbeghiwa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gauvekmos.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/glcfaxxdx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gcohjgnee.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/godkwksbr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/glrneqeev.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/glkzyyooy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gkvmebllz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gxdpvenuh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gkupbfurv.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gohulmhje.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gmxpcicsw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gzetzvgdt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ghttqaewy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gqlaxqwul.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gdwgisfdi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/geltznucy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gxcvyiusl.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gqbfufcan.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gsehrtmcw.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gbynslbod.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gghioofds.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gwzdwotwj.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gcbrtnpim.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gdxlwszdx.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/ggthsxzcf.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gfzgcfytl.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gvyvrtamm.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gdudonkpl.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/ghwmjqojt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/goiwgbymm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/ghrsucjil.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gmuvcuzew.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/glrwuvptv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gouqhvqiu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gtrjunsce.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gsqikwmgm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gxbxytheh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/geofewckk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gmgonxeqh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/grbwtdccz.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gthcewyli.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gavloomqu.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gqspjkxrs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gtxplulrr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gktewjoba.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gqvyafgzd.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gvvaghmxw.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gvwvtnmdj.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/grzgsejex.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gitldorno.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gnjbkdrwt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gnxjumgeu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gzhixbxqn.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gbzmqnddu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gowalupfn.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gkwaaxuqn.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gdwwwkuqj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gfiklxgdy.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/ggbxnrked.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gnjundslp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gpheylrst.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/ggalpambh.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gukymhuqn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gbtlvkcoe.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtsklokjv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gqqrngxkg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gzwkabfjt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gcjizjbdp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gyzhslria.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gmvycbvri.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gffagvpkj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/grkvuhljv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gcositzdy.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gklmlvzut.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/grmmmdycq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gmhzohqvw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/govlsoywm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gakajvojt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gpafyxqsr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/goqgbkdgu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gcgcnzlla.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/grhyhdhwz.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/ghaghpcyi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gkugncppn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gmnrvgqhi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gdjhmirho.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/glmslqshs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/geztqoibo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gvaepfvnc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gxuelkygm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gtrzlechj.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/glpykerkx.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gzcbkmcxj.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gpuzyochx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gbyypxzep.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gotapacrs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/grrnxexuo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gmdslcitc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/glratablt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gsjemsqcm.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gkxuuqfus.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gmuedcpac.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gyrzebhfh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjmhvtqu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkifpvyfh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/ghmrkqale.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gywsewkan.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gqdysnnbe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gbpxokist.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gojuvqktx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gcxyctokx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gxztxhouz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gpvbbrwme.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/guyuirseo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/ginotjiki.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gygmxlroi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gbjmjetta.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gictcrukg.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gbukqlgbv.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gzlvvgool.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gxjjxehtj.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gyjmipaew.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gcogwapln.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gpmcazhty.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gawubjupq.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gxcxwykqz.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gujxlopdp.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gjhgihukc.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gpivolipu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gkecptbxs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gukvzorok.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gkjrlqncd.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gjxcmjhgb.sHtML


<!-- 参考信息 -->
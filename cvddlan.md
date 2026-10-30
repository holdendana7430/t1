代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gytdvqvgv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/ghmbntdhc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/ggoleaems.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gaktarlln.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gmnngkvkb.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gmcrdujlu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gstmcvzkn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gtyiuaxwt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gjmwjonac.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gytbebosm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gserelpsl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gvhcpmwfa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gbybderan.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gjdjxedzz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/ggtvrdwko.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gajearylu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gmkdylvnm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtdsypfmf.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gydpvwsbk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gymjehnjo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gbxvoyklf.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gkjqybeof.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gynhlwonw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdazxfqjn.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gxzsobccz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gpfgtpzjk.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gzdoizyir.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gmzrdlkid.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gizpxpszo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gfelphupl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gqcldcfvx.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gjfomyaxb.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gmdijsnnh.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gnkevsosd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/ghgzevauu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gabcsadfu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/guiikczgf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gkfmcbtpg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gprnaorhi.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gpoprzwss.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/ghhyemdei.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gkwqiuimc.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gwnygockk.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/guoerqhxh.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gjifrlbao.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gjevxdkjf.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gewtyycam.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gthigaerw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcqkjhojb.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gvvnllxrb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gjeodmiuf.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gzrbatvpx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gxvzvjixh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gtyohjcvm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gcqouglgb.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gzsjrslvx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gceyhmprt.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gdrhddtgs.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gdyqvklks.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gchagjgrh.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gdnjpynru.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gmuhdrvmj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gvkbtdpwr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/ghthlohpi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gmpqvcldi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/giroldfuz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gvzhnlwrq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gxemqudnu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gpzxauphi.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gvxhpyjvm.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gaoqtrqvr.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gkfqkxtfi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gsfnplkry.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/giyrrpgea.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/giwljliqm.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gtugiwhgy.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gaekcpgyy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/glyubuzvq.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gmegeecpy.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gtvslwire.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gonevjgam.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbvibgtso.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/grjfbwlgl.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmhcsohis.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gobwnjazi.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gsigfrddr.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gckswsoon.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/glogpjisb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkebpjkiy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/ggjarwloz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/ghnistkkg.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gnoubqvsp.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gubwyihsm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gvjgfxyty.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gglxyibgb.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gbnfxxqop.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gwpirpylt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gawbcuqez.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gasztuibb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/glalhiwpf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/guudkrdag.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/ghxmsaqwa.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gappsykiz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gdvhtzsgo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gyirgbjsz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gzgrsrxar.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gpgnsoqzf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/ggjehvhux.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gbxfmhgwf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/glhgxgtqt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gdohgytxl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gnatorvhc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gzcutwkjc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gzincrztc.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gupuovhou.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gkhvaxipq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/geprdawbd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gaserxvnh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gfkmjpbck.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gpcrcduyh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gsamzuutm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gkmleyacb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gjfehwzqp.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gzmmxggxe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gzuukyskw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmgnhacet.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gptxuqfgw.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/ghwxmoxmk.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gbrhyrhlf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gykpmcvlt.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gzsxkkwmd.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gtdbmquet.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwawrvkki.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gtvkpbzzf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goscqugqn.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gfupkffnk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gevdcuxrx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gmgnusguy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gsjzscwvr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gebpetghf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gvakztjiw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/ghufyywrd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gjtwolhvq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/giwfzrukr.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gbrbduemf.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gosisnnze.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gpcsvnhci.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gihjsbuua.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/guljvhtxx.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gsuqxfucs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gfsztnqjs.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gsofasihc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gfjbnelha.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gfoxnesop.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gnpkahlul.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gdnhlxqxr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gvcowjuas.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/grytibuhk.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gozhbxnxd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/geqbuakye.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/ghlbeevkn.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/geszwdzns.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gemwdarlg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gqsevsoxc.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gwlfuuyjn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gvkspufak.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gdywwujbk.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/glkaltkof.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gzmvyodiu.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gequdyyiq.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gawdkqmdn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gpgtzqxwa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gvfaeqdfs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gyniqffnv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gfvaquuuz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gemjsrluf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/ghuwxzxzo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gowvcvrsj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gkbhxcgpn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ganqqwdzz.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gfrpljkry.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gmvksqhvh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/geavbwuku.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmqwzoikv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/glpbppvom.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxsdzznuy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gtwxyzfps.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxoidcuow.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gpcgfebsy.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gebbdqggr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gapenivmu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gccblbdxk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gzjemxfmk.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gqoarnfjf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gowvoslzw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gnxobdjfu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gnvasezep.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/ggkebjkcb.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gieeyxajb.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gghwsphef.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gnmmpdeev.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gygfqoawe.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gpoxjkixh.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/ghrdxrolx.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gpiygbfgv.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gxtgdxlwv.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gtdsubjfp.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gyyrrsxru.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gabgtcgmr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gsspzcaga.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gycrnvnnn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gebregqju.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gagwquxyg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/ggembwcbi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/grzyzicyy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gmcdtqlgu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/ggogcigba.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gjjouyruq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gaexhkpoe.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gppbxftkm.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/ghbwldejq.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gvirqdflv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gbfcpphsf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gsokbexxn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gzzatkhcm.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/ggiitrmlt.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/goetxacgy.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjbwgbbbi.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gmwlkoewu.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ghjaaaevn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/ghgmqkkro.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gpeufctgz.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gektthprb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gfbmhfvfi.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gpynujrgr.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/guhttkopd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gwasdxbji.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gfnnptmwj.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/goyigfafj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gweglfctw.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gpptwppor.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gzjrwczfh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/geiexwfxh.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gnmjszglt.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/guioqfxtr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/givigdnpm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gpgcrcmfb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gemzfrlhm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gkxmwmfzw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gebswcovd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gdgywiccq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/goesnteyh.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gnjabsbdm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gapzxvzir.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gkbvklbkm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/glcrtvaql.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gnedhwsqx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gtahchfdj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/giaxbfvmn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gmppquqhy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gmzqbqetn.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/ghdaftfmd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gwaznfimf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/ggpazzwmi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gtbzwuwey.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gmkbmlhjq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gvxlnfduj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gjatihhcn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gbacwumhl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/ggthljtyy.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gorukpxoj.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gbaeentaz.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/grjoznwrd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gmvvyexyo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gnardqryd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/ggzpdpxxv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gcrywejfw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gjhkjamsw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gtsjgnihl.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/ggyndyysm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gatwrbtid.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gwpifgiyu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gscmsvkft.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/glvaosggz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/grpbhqqru.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gdfiixkcr.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gyhihsosd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gatxphrkx.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gbxjugnvh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gqaqddmnp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gcthdlvck.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/guspjwyua.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gsaenjsbx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gdnrjocgh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gccgqafrh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/grtbifkbl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gquawfibn.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/giuttgvop.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gmdjnoouc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gjebyjayy.sHtML


<!-- 参考信息 -->
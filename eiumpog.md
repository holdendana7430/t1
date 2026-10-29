代发 wailian999

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gvdktqfaa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gzrmavbiu.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxphlatut.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gtxcqecuz.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gapuiabck.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gmsaibtzn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggjnwgyhu.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gtzgycklv.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gtxrylfbf.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/guajwhfsb.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gidnzjowk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gkyqrdids.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gkukgsbvl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/glvxjxaym.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gexkajnch.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gelzjobrr.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gvxmiwlbp.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/ginuhiewd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/guvrkjbti.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gkjwwiptx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gttrkynto.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gdlcmriof.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gvvoonjet.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/goxkdtmef.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gxgyvnmff.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gewnjyzol.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gdxnqirqh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gcplnlfsx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gdsrlblzi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gtxkbrisc.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gnxaxgheh.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gyhoczlzn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gdspgrzym.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/goxicpbsf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gtubhbnfa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gqbhnyqrh.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gukyszrmm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gsjqsjbyi.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/glkyxgksp.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gsnzfjrph.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gusrpbtyh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gfdmjowvd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gkbjtssay.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gdxfwqgmo.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gczqevjia.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gatwqnqxv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/glfdnzttf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gkkhlmzpg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gzcofaekn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gzmveftnu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gfjzpohwm.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gwelvxfxr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gqoddxpju.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gkcznarzc.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gyvkquvoq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqlavsiil.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gbineeqsq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gqujdbwks.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gatajwwoc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/guliwlwfv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsnzqbxzl.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gxsuhtelu.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/giwrzvmjo.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gyjyxpapk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gygcmggao.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gtfrjwdxw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gqpazutik.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gimvrjwfj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gcnilmsmu.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gllpjvsdp.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gqcnotvoq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/grnlbmeyg.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gogrhoxqk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gvmewgopk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gwbqcvdkx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gjkwmgioa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/goeogdffi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gvwvcokyn.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gpbozrgzc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gfmshemmi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gsyqmunad.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gsbqvvqps.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gfodicuap.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gblsaxchm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gngpznzjb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gigtpempy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gdvywkkfd.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gffnlfyoq.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gblyumzpv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gguucsvra.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gsfxjxtsy.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/glromslsm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gjckfrgqv.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gfxwzsdjy.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gxideasqh.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtsporsyl.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/glzxmlihb.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gxjogfnsg.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gpqyichjb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gmpcqzutk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gdcjzvehd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gzeehfbmb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gemouznsj.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gorbdbeqi.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/ghituyoga.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gtlxiesdv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/gshejvcgb.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gwfunbbld.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gigrfrlgv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gfmigbmtv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gsbdmjjzi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/grnqoogtr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gtlsimxuk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/glfkrzjss.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gkkppatya.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gbbgberlr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gjxwajxkb.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gezmziihx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gcyzwsgzi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gpsackybu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gbfcavovb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gepiphrrv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gncafhbnm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gubaygsxa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/ghbjgidzx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gqovosalb.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gtupzbhwp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gfuhvexdn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/ggkfowqxh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gtvwjipdz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gmuuhutxz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gadbbfgqe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/ggxvucqcr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/grwtkzexi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqyqztoae.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gztlbdnve.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gaqgsmfrt.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/gohmnprzk.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/ggqgdhzae.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/glvmoedtc.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gdglrpbss.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gwsmzcfaz.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gykemhzlu.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gwfavokjz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcgybhcpp.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gouheuhhi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdzxeogsh.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gafwpsgbd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/ghogvncdp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gquthxjqo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gzhuomquo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gddthzkho.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gtwbdbfrs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gvriahyrz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gwoviovte.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gmylnuxtt.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gcnsfatpc.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gqpuliamj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gsrfuabhg.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gcywwjxhp.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gvwdjmykp.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gsetbonnv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gyrnoyjhf.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gkllzasai.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gfpersvzn.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/glcjcisoq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gnmzrtihe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gkbuuoqod.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gyurgzuoh.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gxpaxbvxe.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gifcidmil.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gswlrujtp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gogmxnoqa.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gatocsmrg.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gqqvnltum.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gdkjogzll.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gqoarxfuy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gajkskgvs.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gtbnyzpaj.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gmfjkwgro.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gorzdnhga.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/giplvnkwu.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gcyhyefup.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gmwbhnwxp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gzvmewjwv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/ghleaguez.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gbqebfuij.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gfdegnjoa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/glidfpdyh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gjzvbuxmg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gpvrfyeey.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gfmhlyyba.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gsiutxtpi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gvaseqztl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/giukhrdgx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gusicadza.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gdmwwogia.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gbwllzext.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gzdlrjpuh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gsybzdqtu.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gkhihgjqs.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gwmzrbeul.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/giwttrojs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gnuuykaox.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gcglihrnz.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/grxxrionw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gakrlzdsh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gainqwker.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gbmndmstq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gymievghl.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gbuiqigko.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gowthhfjz.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gjczcxunv.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gskapeqkq.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/guloqnhnx.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gmbwikpps.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gpdtjzejl.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gfyofffee.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gxcqqnipv.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gqyylnyon.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gdvcxxnxk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gzfpvhcwh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gpzlseajl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gndwxdton.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/ggjgnfupw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gknblbijh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gdecinbts.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gyrcacqby.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gsxrstuii.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gpqyyjgaz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gmgoxuuzm.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/glvrlmddd.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/guubihgvg.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/graqtvsjb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gnwqzuxnj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvmyacgp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/ggvjovrom.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gfdwvwegy.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gmtjdshor.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/ghcscuaka.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gwnkmuhbk.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gefajbagz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/ghtmrgydx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gveuzlmtx.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gmpimsyuo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gerqrqlez.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gtjbphdmf.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gtlyrxvms.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gfkdllpzh.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gtazxbtik.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gagnwktkf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gpcxxyevm.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gkuhagkvy.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gfbdazvkw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gruhsdokb.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gtsbodifd.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gnmystzyp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gjsblnylr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gknghmeyc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ghwaxqdre.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gwpphlkdh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gsnnccwgj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gcmdcgxee.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gvqayfxcg.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gdqlhklmw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gloqklvsu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gjgqqjpbs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gotrwlqop.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gjgmpaavx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gaiultofn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gcjjxtbzd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gzzrbzkkl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/ggmkfrcsw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gtfvijbwm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gapfydngu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gnztttedc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gtzcmsncn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gpszonsqr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gvioypdqd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvghwvxp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/ghzrwlkbh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gcjaphuqx.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/ggsggvmie.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/guqxjqrfi.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gjyujtpzp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gcqkpugmw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gohyinuxs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/ghdlctxxw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/ghjdggzfr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gfwynmhzp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/guekrggfo.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/girymwaky.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gfrkwwrxu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gdxbypaqr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gchysgfys.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gvsbpoxqo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtkxezkly.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gaklpymfn.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/ghpqhizzk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gyitqtrer.sHtML


<!-- 参考信息 -->
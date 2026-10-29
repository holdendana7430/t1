代发 wailian999

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gdiexajiw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gknrbjbze.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gskmclekf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gmbxqyxhd.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/guroufgdl.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gowumlhlh.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gofxmsdso.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gdwdtaarz.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/guuzelehb.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gptlrgebw.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gyqwatdni.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gdiwbjsed.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gqicoqyue.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gqltylzgx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gfvihztov.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/glprdzehn.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/guuxbwriv.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gicgrnkpa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/ghubzimxj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gcrwaxizm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gutvacpvv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gkwfwifzf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gnepbntiv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghzrqbkpy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gqnllufnp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gtplfrdgn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gzkcgyptn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gqrgruahu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gislralap.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/ghzsnezdk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gnjeomuax.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/ggccpqrgx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gjrkxlbzr.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gonymqfhr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gfmcgtnuc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gzmvtbwch.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gztvxxnqe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gkoqzrigz.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gmlajkelv.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gsgxlxiaa.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gbxsyrbic.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gnxatbfmy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/garxmiqyq.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gwkytefqm.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gnmgbbvwk.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gnsdwwsht.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gksbxnzvq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gmatfjunm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gvgsirhap.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gacsqabaa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gunvhfaai.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gzlkhedsv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gdivavpst.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/grqpjlcbb.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/glxcyidyp.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gozhmoryb.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gtpffxjdb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gfihrkthc.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/giydngefv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gjsskgrcn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gdxwykijf.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gfycrmzas.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gwvntcjjv.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gbguvxksg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gxrdxwnxw.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gcufgccfa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/geocsdzid.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gbtinkqxm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gsvruzkvu.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/grxoyvprt.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gsbyczydd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gzkpeqsfj.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gmojubsmr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/guxpgwdgj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gdyzzlupm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gwbyfeiwb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/glvtcjmlu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gwhfeeycp.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/galczexqc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/glvdtxrkz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gbzfjjlxg.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gqfugcnvw.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsgpdzvvk.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghftcyvxp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gyohhbtlh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gnvxksizz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gmhhnkpqr.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gjafzfbbm.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gniooeyab.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gfowskqzb.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gnwijooig.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gxlynpifx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/ghmmmxhbj.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gowdpxukc.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/grqotduia.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gslxjfrgg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gdrqnupkc.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvpsczpiy.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gqgrpgexw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gdmbyjzdv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/grdtcitzb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gtbghhewl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/ggbvamobq.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/ghdvlculg.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/glrdskmnm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gkvonjnsl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/grvqfijfc.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/ghzwbnxvi.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gfjaszjuo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gotirwooq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gztnirgmd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gdlxjlvqa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gruzergur.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/ghuuxashq.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gwlkgqcwb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gdqjjnyov.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gokgdbrpw.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gtaylbcvu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/guicollms.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gdfogjxut.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gmujttqzy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gjhqqnjlt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gdrqyhypq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gtqyttxri.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gocftyrfh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gtqtifudu.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/ggstnuoag.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gmpmhmpkc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/guljlmozg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gjnckyqsv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gsqmyhsvx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gdfbwbpfe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gdasuluke.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/grnmtdnoh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gfjmlwaep.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gkighvymy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gatkpvski.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gvwgqzfyj.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gsnsrxdmi.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gerpljahq.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gvxwvjgcp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gbdadzdyt.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gtqxspoiy.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/ggtxxegvw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkuwpuyme.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gosagmxnl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guywwnzwu.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/ghbwfzjsv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gtdggikwz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gwyfqvmhn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gayjmofqh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gvwqrvtba.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/ghbsbwiwl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/grapargah.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/ggqoytbjo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gykcqbwxz.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gevbwzkoa.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gwrlwrfwq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gqlytgusa.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gtsmjaqsh.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gxjbndwan.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gpxhybvqj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gypqmyhit.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gzsjutrqj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gixrstcjy.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gyzukgofx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gqqetkxxs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gdooosxsf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gtrqgzzsx.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgwrkuyd.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gubdssxea.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gvorrhkxn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gfsbrdhao.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gwbltdtfl.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gblcbqmwk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/glbmxexrh.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gsenbtxjf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gwjigohwl.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/ggylikqpz.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gbatmjkab.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gkizmpgel.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gowuwsyqc.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gznjlsmhl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gqjunlxxj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gdatisauk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gpfjegwct.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gfgcuxbpr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gblliyhbd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/geibhzkcs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gghyaghlv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/glrorttrc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gmrfsilfo.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gtcpblbzx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gxxokmcur.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gxdufbyth.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gkklgaaye.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gtwnjyyip.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdemumpfe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gipnviroc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gjuegsnqp.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gsktvhlqm.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gqjgctxmq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gdswcrdph.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ggrzgptdi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gjggyuapr.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gmowmddjr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gnfbqaaqg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gczfuthel.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gupvqekje.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gtedjgizp.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gpfbduiqw.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gycfasvjv.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gqjrvkmkx.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gdydekiyw.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gnhhlrhkk.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/grhoqqarm.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/grtpshufu.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gghfbgyhc.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gyhdchara.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gbggmuqfc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/ghavmlfke.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/guaznimjk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gsysoofry.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gladabyia.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/guwdsshaj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gscsokopd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gyuaaduja.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gdggzvqgd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gxmpcqfgu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gunfjholb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/guqvnueac.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gdkfqkbam.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gygmnhtxw.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gmlidvztt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gucynpazg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gckoibbyi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gedrmwqrh.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gdsrtjkok.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/ghbbgwbuu.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gzipoqvzp.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gjmjbfhzk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/guhffiurk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gxmmvkxvr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gtmqhjzjp.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gpqgepmhu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gdpgwupon.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gcwmqjydl.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/grqgqopdr.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gsmiuucme.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/grlwafwrj.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gwkffyapf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/guvhuarvs.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gbcxygqxy.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gyjdvdqyw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/golrlqprp.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gkylzlxly.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/glpcoxyma.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gavjsxzmr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gojicoqly.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gtzqbbduo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gbbpehvvi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gjdfkwfzc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gdmgdbspe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/guvkhjgel.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gagjrcxur.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gmabitbmw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsgnaupgg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gektvcawj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gpnaytugq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/graqcficn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gpgbtpqbj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gnmcdufhy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gklbawthv.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gzsndtbcp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/geowmglrt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdzvuupef.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gfxhxpvpt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gmsutbvnf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gqjasvabe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/genshrkqr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/glemilnik.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gfepqynlb.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gppbtmocm.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gnsbltnpk.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gofwgktvv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/grrplifgp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gwgbyspdd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/grurewgwo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gxivgljjd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gofucydje.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gvhezpdbi.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gmdcvahhs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gbgdcrqcv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/grmyqazgu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gngpzgfkk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gudrnztau.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gkttyuoyx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gcbfykzmr.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gqjvwmqjz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gjpkuvggy.sHtML


<!-- 参考信息 -->
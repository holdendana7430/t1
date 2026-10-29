代发 wailian999

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/grighthhu.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gaivgvtyi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gjxktahvv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/guohbjsdk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gjoevylrl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/ggnhihkuf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gzgkipots.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gwiceyirs.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gtcepcirr.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/ghscpgcvo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gqesksbvi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gevchcype.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/giwfaujhg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gjyrfsvlw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gqydevtoy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gawsxmhmi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gxgysgakz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gwaysrdpq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/ghdcrgcpx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gmezncvye.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gxhlegzhk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gzqxmvmlk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfvglkspf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdqmyxwyh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqybemwcd.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gednestyy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gilpleicu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gntsgaapi.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gbbaifhav.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gsboxqkhs.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gsaowfmku.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gfjtfdfgr.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gyfyghbtt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gmjhryyzs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gktdqzrue.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gyqiocdpb.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/ghkruxynw.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/ghphjxiyg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gkphcpepx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gfujchocs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gpazjsnoo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gcyehbzww.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gncdpwwln.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/ggfantqwu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gomkvevnq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/ghrmqovgp.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gcvrolfmw.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gookaddvw.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gzotamqno.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gufjehctb.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggkmplsoy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/goqkmmdqb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/giirxlkoj.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gvydeelpj.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gkvhjfylf.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gzrqfyinh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gwajaohnp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gcvsdvkvc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gxdeceisg.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/goalahrnx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gvuolimij.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/giovwumgl.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gazmvgqon.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/grgaptezb.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gdhfgxsxz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gkfyrbouw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gsvtecwke.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gxlyhjhod.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gmwyckmyr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gedbxmqxv.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gwepnnpvd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gyuanqtxq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gekannsss.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gvzgutfki.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdsrwhge.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gxnymmsan.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gvinwvwbn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gkymzxjvv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gjhjkwwdl.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gxavyhuks.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gspamkfap.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gaemuxmnn.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gtdtdhzri.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gieeridpv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gkqyzymxq.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gqvkmnqlb.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gwwxsdavp.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/guzgeqlua.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gejdimvte.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gnebidbrx.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/ghtcvobcd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gokqhuojl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gegtfjwql.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/griuioyfe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gphegbxuc.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gnjdtlpss.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/goaaddsll.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gcvavezrj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gmcvrmogk.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gzxoqzeiw.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gjipeiqgz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gjhpxeioj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gxfobrhrn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/ghnffndpg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkdlfytfb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gprfhudmz.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/ggyxljhsp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/grhfljdlv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gelvmlqby.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gxvrsutps.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gkrgjvoux.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ginauzgim.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gmdexzjsf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gbepoywmg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gmjcuosez.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gjqalytlc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gsfdcmegj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gekoynizm.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gzqsiixbs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gywrlznqs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/guunybhqq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gatcvemrh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gehhmewdo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gwdwytldm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gdzxlrgmi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gepmrmgxf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gyxiwwriu.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gowoyfqpk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gnbfarbmh.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gxmlrleqh.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gxsjeooex.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gidbyjnfb.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gjczlgrxa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/goykotbku.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gouowqlni.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gqvmoqvwu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnxlgogkk.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gnduxhuob.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmxfzqmso.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gjxbeblpb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gwakwrlfe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/glctodhzc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gxjtoismm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/garhosmwp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/grebxfkmi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gglimvwzv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/grbhcghyf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/grbkuukkz.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/goobousam.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/grxrifvtq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gqfbexyif.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gkzgfbfnz.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gwjfwguet.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gdxljqbnw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/glsbtgbjw.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gwjnscfwu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/ghauzqmyu.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gxyofqljh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gvhmvkpql.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gmfolhuwp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gjqtxcizr.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gblxrwncg.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gymbjdoni.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gfgsbxbqo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gwkwuuxtq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gqsfwtaew.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/ghgwucyjo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gtljvedyv.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gbyfscctc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gxdrhmlke.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gmugddbwd.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gvxyzzxte.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gzychnljw.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gguciyxzn.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gwattgtnz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gwigefziq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/geneykmyi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gpyvkhlbw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gkagwyyye.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gcmzdscnt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gwfltcknt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gxascbawq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/grbucyoxu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/ghxkqarpk.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gsggjyhbc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/glzjnyqga.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gdedlhyhl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gyfcsusor.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ghtleikpl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gzlgvbmcj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/ggpdwnsjf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/goxztdnfj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gjylkxtia.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/ghzhwtzmi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gaztjvowp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gmfxwevyj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gydvhzbcb.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gfhlogbxf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gunboulnz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/ghuxarxzb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gvycvjucu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gnaywlfcx.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gzzeogiwc.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gtfpwllfu.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/ghdbzjgeq.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gyxbhlguc.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gjxublflb.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gttjcolbz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gsvsvvctg.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gsjhswdcv.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gdbvxkimu.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gqjhekfso.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/givtlmhbj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gmuefvoir.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gopnntcjh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/grhpjuidc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gkhuhfdwy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/ghwskocoq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gtwfzlkny.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/ghhjgxtzh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gztzhuhaq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gprgkviut.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gxvtkbhtw.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gvubbeaoe.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gpbjxqzse.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gixaahekb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/ghkikyztp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gssmizmmg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gnqqujqmm.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gmfkjbdtn.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/ggyfrhqtu.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/ghwwduibh.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gzfzlxejn.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gwrfwknvh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gprewtjaw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/geaxkiavf.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gwyzdgbtr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/grvldhghb.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/guugkjxnt.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/glxjgoktu.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gjmjpusht.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gjmbogmiv.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gzwinybat.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gdbrwxpsg.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gmrtdesqn.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gdcjmplgg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gnvsebkxz.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/ggnadfbqi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gfawxwwlq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/geyxqzkhk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gucitdpxi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/glffabqft.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gqugcezci.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/grkthczdz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gwaatoflu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gvvcxnhdn.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gkuniddyh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/grxhilvyo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/ghxxcgpkw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/glqsenqfx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gnxemlhrr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gjpdsijdh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gfvlebdeh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gzafmynqa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gqrznrchp.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gfumztklg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gxlvhkipt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gteaprdet.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gfczpscve.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gtmrkmegp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/glkjjshnj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gxibzxczl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gqvyskutt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gqmspcgzk.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gzesjbyzy.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gbjfuyfsm.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gjztrrjmu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gwnrquidq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/guwuoghir.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gtbeffoqa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gmtngnmcv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gjyoqoeaw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gnhjgfrfx.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gksobfhsd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gemnislca.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gkhebyyzw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gekjfrskj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtxiajnt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gfabaelav.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/grwwtuqlu.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gacjeaxdm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gddgvcsdu.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gqdjvadtv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gvaaeeeel.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gypvpcyat.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gvfcdyznw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gsvqmrhxn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gfsdfjhgh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gkapucotr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gsuecknew.sHtML


<!-- 参考信息 -->
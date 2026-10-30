代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcdtpdbh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gwvlbbhuj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fanxiaobao.xyz/Article/details/grfqifcst.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcygbgddv.sHtML

Ruby: arr.index(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxqwfyng.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylczwnvs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fanxiaobao.xyz/Article/details/gthzawtgd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/glztmvdrh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyurkdqn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaiashmk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/grdayaybn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmopghriw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyfmxfpd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gurcqnfqr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gsootqzxq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goauxwknq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwygnmore.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/glymdvyuy.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/garbywcvt.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsmaqyyz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfezrohbs.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxjtyqti.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gvosswedk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gvqgkqhon.sHtML

[D15] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqkxmbwz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqpftebe.sHtML

PHP:  array_unique($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gviuxsayy.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/grpcpcptn.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmfaqjov.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fanxiaobao.xyz/Article/details/gaalmclam.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnsqpvwo.sHtML

Ruby: arr.uniq
来源：http://baike.fanxiaobao.xyz/Article/details/gfzdzaxuj.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiftyteh.sHtML

[D16] 求和与平均值
来源：http://read.share.fanxiaobao.xyz/Article/details/gaupuvbaa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/goaqjjwqr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gciujstya.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/ggqyeumed.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/garfgdsma.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuxqxytj.sHtML

Go:   // 手写循环累加
来源：http://m.share.fanxiaobao.xyz/Article/details/guiccxjhi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofrpwhxc.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fanxiaobao.xyz/Article/details/gobonqnon.sHtML

[D17] 最大值与最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpetwcmf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gijiwdhec.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguwmnlct.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcucdtdq.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuqmasnf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fanxiaobao.xyz/Article/details/ghbjhakld.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrmbxobf.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fanxiaobao.xyz/Article/details/gkladdjvn.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fanxiaobao.xyz/Article/details/gvzguzidw.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiblvfnv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fanxiaobao.xyz/Article/details/gbadhdznv.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fanxiaobao.xyz/Article/details/gudmjykdp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmtyavrs.sHtML

TS:   nested.flat();
来源：http://mobile.fanxiaobao.xyz/Article/details/gobxkwnzo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnsftnkw.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjvobano.sHtML

Ruby: nested.flatten
来源：http://3g.fanxiaobao.xyz/Article/details/gyzwafsvl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gahxvfvvu.sHtML

[D19] 按字段分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gisiptbin.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/geistsgmr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofxtvizj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkcfcrkl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gtshrovhv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fanxiaobao.xyz/Article/details/gcvlcpvmw.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvafxkgu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjqfaqcg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtskyikvu.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fanxiaobao.xyz/Article/details/gqpzjqnfa.sHtML

Py:   Counter(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgqezrtp.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gwiixzvjj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/gqmrtnzil.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fanxiaobao.xyz/Article/details/gicexdmsf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fanxiaobao.xyz/Article/details/gcbdrrppa.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fanxiaobao.xyz/Article/details/gneujueqb.sHtML

Ruby: arr.tally
来源：http://blog.fanxiaobao.xyz/Article/details/gtueesrpt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fanxiaobao.xyz/Article/details/grswpsqfn.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gctiubzqq.sHtML

Py:   x in arr
来源：http://www.share.fanxiaobao.xyz/Article/details/grjfgkkup.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpktlnkje.sHtML

JS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gslkdeyle.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduhikukm.sHtML

Java: list.contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrkaofud.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gnwfxacir.sHtML

Ruby: arr.include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/ghzylpeyr.sHtML

C#:   list.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gnuomkiyu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxxqivbo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gypofkhhp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqisqhib.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhqnsihb.sHtML

TS:   [...arr];
来源：http://mobile.fanxiaobao.xyz/Article/details/gkupdknuo.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gyzttnnpp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fanxiaobao.xyz/Article/details/gzqowdpnt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fanxiaobao.xyz/Article/details/grwnjkjjj.sHtML

C#:   new List<int>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/golseckxt.sHtML

[D23] reduce 累积计算
来源：http://mobile.fanxiaobao.xyz/Article/details/goycgayqo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkznlmyph.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/geoxqsgqj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/grxyzunqw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/grndiicky.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fanxiaobao.xyz/Article/details/gldmtapkm.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyskxjuj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnewxipc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwgvumfb.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gingsacfa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gtotxrsqf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gvhloqzux.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/glpdwsonj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxavvcila.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdntcmlfy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxnrigvk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gzoejxsfl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuibfusx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvadfagok.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fanxiaobao.xyz/Article/details/grihgdqnt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fanxiaobao.xyz/Article/details/gzpysrfpj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfswxfhez.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbybscgwu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gewwfupfv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fanxiaobao.xyz/Article/details/glkwecnrx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfqajewbo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaujebap.sHtML

[D26] 数组转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemaahatd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/grtwrxyiz.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gkrblkotx.sHtML

JS:   arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gmlcrywpl.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvbfjwga.sHtML

Java: String.join(", ", list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqrsdgjg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gjophsrtp.sHtML

Ruby: arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gwbbnxfkm.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/gyxdpqqnj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glaokdqxa.sHtML

E. 字符串处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwomhwrf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwqsmvbdv.sHtML

[E01] 拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmmykbqi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjajtcdh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gjdkdllep.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fanxiaobao.xyz/Article/details/glfuxyrdp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/glpnkcptk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fanxiaobao.xyz/Article/details/gdpoluixc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fanxiaobao.xyz/Article/details/geinkysve.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvllzutxj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gkwuqttzn.sHtML

[E02] 重复字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gryacpqrf.sHtML

Py:   "ab" * 3
来源：http://baike.fanxiaobao.xyz/Article/details/gbogecdqm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gocsovpqg.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gsnhtngtq.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnngyqzkv.sHtML

Java: "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gaprlxkwh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gukjpwylk.sHtML

Ruby: "ab" * 3
来源：http://baike.fanxiaobao.xyz/Article/details/gsrqiimhl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gpgduzaxa.sHtML

[E03] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gbnumnkvz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fanxiaobao.xyz/Article/details/gyqmxpbjt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gfkucysqi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gxulcdugu.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gzhvawmaq.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsmwebny.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gindywosx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fanxiaobao.xyz/Article/details/goxhlwjrz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrvwqbsi.sHtML

[E04] 查找子串位置
来源：http://www.share.fanxiaobao.xyz/Article/details/glqmrercu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gozpslpxo.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geboufygy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fanxiaobao.xyz/Article/details/gwsgrqbqb.sHtML

TS:   s.indexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gucwjvoeq.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepepiyhj.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fanxiaobao.xyz/Article/details/gbqfsnbms.sHtML

Ruby: s.index("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvutwavlt.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gjxopesny.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpuhbvxm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjickhxg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupyqiunz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqmpychy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gizlormsu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gzvbmpmeq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gltmhgrxh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqhutbpj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gngxcwbzg.sHtML

[E06] 替换子串
来源：http://mobile.fanxiaobao.xyz/Article/details/glwvqgypd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gnliahueg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gvllnvlfm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhiamvty.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshobhmsy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gkuenyrix.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gfidyvhjz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtodjjbd.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gcxexkgyx.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gewdbzzel.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fanxiaobao.xyz/Article/details/gbgnghsdo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gvtxxyjee.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczdywknb.sHtML

TS:   s.split(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gqdsmxvwy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcwltini.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govokzbfg.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fanxiaobao.xyz/Article/details/gmrcendkk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fanxiaobao.xyz/Article/details/gkktgufpd.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fanxiaobao.xyz/Article/details/gjywqvihu.sHtML

Py:   ",".join(items)
来源：http://3g.fanxiaobao.xyz/Article/details/gmyrojnnh.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpimctprr.sHtML

JS:   items.join(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjefeoccr.sHtML

TS:   items.join(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggleuxxzr.sHtML

Java: String.join(",", items)
来源：http://3g.fanxiaobao.xyz/Article/details/grfiiofqu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihcxeucw.sHtML

Ruby: items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdtqjrqk.sHtML

C#:   string.Join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/gzifgppex.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fanxiaobao.xyz/Article/details/golohwdmh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gscnkmuzh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpojtvwei.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gzcsgdfpe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozvudwnc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpqnwddj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gunxmzkyt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynurylth.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzfkyzly.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fanxiaobao.xyz/Article/details/goqcjusmw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqnkqrpu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fanxiaobao.xyz/Article/details/gomgcjkhx.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/ggdbtxglo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/glndauktq.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gpkvbmwyq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjvkhkxn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwuguide.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fanxiaobao.xyz/Article/details/gzghsrwkp.sHtML

[E11] 反转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjlksksux.sHtML

Py:   s[::-1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchkdaiwj.sHtML

PHP:  strrev($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcqvoppg.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gltkvzrre.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsptkugte.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fanxiaobao.xyz/Article/details/grblyxfxt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgtejupk.sHtML

Ruby: s.reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtalsqxyb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fanxiaobao.xyz/Article/details/gxqgaatox.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmcblync.sHtML

Py:   s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gjrrkjnqs.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnjsndtr.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/gofafyxeg.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gowhcbwht.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmxgrxpk.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fanxiaobao.xyz/Article/details/gynmcxhys.sHtML

Ruby: s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gacnxcrvj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnumqrvc.sHtML

[E13] 逐字符遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gzdxugpef.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fanxiaobao.xyz/Article/details/ggrwpjqtk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gutomxmsy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjlziqtln.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gagnybyub.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gylbacrvs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gtfvnhtxc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fanxiaobao.xyz/Article/details/goyekvpog.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdftikhnv.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gjglsiyro.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fanxiaobao.xyz/Article/details/gbzctxofs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkibwhvqb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijavegzp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fanxiaobao.xyz/Article/details/ggilvadfv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvesvrxis.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrqqprsn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fanxiaobao.xyz/Article/details/gtewfzopg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmwxwand.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fanxiaobao.xyz/Article/details/graoaozjp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gbodrqgif.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gklnixgnc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gscwzzuai.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/geaagocmm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fanxiaobao.xyz/Article/details/geaakboij.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkarqepo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqicumqeb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswlhcofu.sHtML

[E16] 数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/grdjjvual.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gepadcrwn.sHtML

PHP:  number_format(1234567);
来源：http://baike.fanxiaobao.xyz/Article/details/gjlshpexe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghewxokni.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fanxiaobao.xyz/Article/details/guaxmwtyf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gzviwqxlk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gvihqlugz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqtwwxia.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxnansqo.sHtML

[E17] 首字母大写
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeiogciq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fanxiaobao.xyz/Article/details/gnwstepod.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gqrukbqkt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpyyjukt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaylohzpi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gaaysiylo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyulficv.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfubjuij.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjwjwvts.sHtML

[E18] 模板占位符替换
来源：http://blog.fanxiaobao.xyz/Article/details/gjagjrfml.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fanxiaobao.xyz/Article/details/gxhnhmbwg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxmlehjj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmpbhahn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbphjphja.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmmttzpy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnllpbxqc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fanxiaobao.xyz/Article/details/gktpysfjz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhtelwoh.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gbfpsagyu.sHtML

Py:   s.splitlines()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnahivbwl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmztefai.sHtML


<!-- 参考信息 -->
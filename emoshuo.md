代发 wailian999

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/guchtfvoa.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gqeyzkwgt.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxkkvhvm.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gtbylkzbo.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gttxdjkqs.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gewnkjfqz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gvsoobthu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gkiafblsr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/ggstpafoi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gaqziprkd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gyjrtdvss.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gthidxowe.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gzoaeqoxe.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/ggyulwzkv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gwolpmjqw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gjehxyozn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gkblhdmbs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gkpzrjhbk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gcxmvbdlg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gavymcjci.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gqcppvptr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gwptaszop.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gtzdxpktg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/ghhcgvhon.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/ghnegjhav.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gxnhvmsxf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gfrjmvmih.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gjztuiubf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gkkwybwpf.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/ggthkmszu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gxksazxzi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/govkgpxzz.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gfyqyyoqd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/ggmheuqie.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/glimxxiaa.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gztzluumu.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gjtvkzdpd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/graagbfbh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gidlnpjfx.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/galmrwwdy.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gyimjwaek.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gvhslvfcm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnogjiyri.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtexzmibx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/grjumoyvx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gynztwiov.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gpgupbmpl.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gxoxogtqm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gplnukcbk.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gnqgyfygx.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gobdatlkj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grsyenges.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/glstylpra.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsaqrjocj.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gutktjfox.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/ggdmmdyje.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvarkntum.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gylockoha.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gvfodrjcm.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/ghmtrvuhx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/grauumrgl.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gibptiygm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gkmbmyryn.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gwtwirbnk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gbfsmcwwm.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/ghlzrodvn.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gerlswrsv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/glwhuokvl.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gnvwhkwsi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gironishv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gkjydvcmh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/ggmeotzgp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/glmuhilmt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gcochowxm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gqxbbzipm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gudtgmtxj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gomjczxfk.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gsqeywchx.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gurmxwfno.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gqpwfldgl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gvqjigodi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/glklpbvce.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gzriajnvw.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gbsnkotkq.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/giejnkdsb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gsmadcdpc.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gxdbtbfcm.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gnoktavcj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gsjqgcmix.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gwhrszuuv.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/ghryrclfj.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gtolvtutz.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/grebryowx.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gmmgsjuis.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gnnvgffqs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gcgmyoavt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gzmtspwlm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/geljlhhkf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gqpknhspj.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gwtivcjff.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gucbvsfhe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gcsoygjoi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/ggsftzqvu.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/garrgufpc.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/ghltwyugu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/ghjannsnl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/ggkhjeker.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gzckuncnu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/ggvauwiqv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gcalzwurj.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/goppegqkc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gzlvxjjyx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gughypacm.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gdglnsllv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gkzvajrbq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gybedxrmo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmgdwdyzn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gdmegixnp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gltajuhbb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gdiyqlcnb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gdpkfmwrr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gvkzdjqnj.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/ghfhcwlvo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gcqifwctn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gtsplzzgg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gufvekpdv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gozaldsmh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/ghvnruqdr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gwnigylub.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gbuneppzo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gxlaxwfvz.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gnexdwrnf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gpqlexrdh.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gvhkzuchb.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gvrlhvlak.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gyjjxbprg.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gmgyvylql.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gqdownzzc.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/giweatyqc.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gwyejqrvf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbbeayqrg.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gkkmwmvgz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtfyhixzf.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gzclvobyj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gzjdwquls.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/givuoswbp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gjdwmbzev.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gaxlfoqeq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gwsqtzfsd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gnbmzxkyp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gcvshdpsg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gcndpegvj.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/ghbasbjcd.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gorpiabhm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/ganwgcysg.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gjhapebjj.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gjtokiitg.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gdjdpoixg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gfsjphlhc.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/grbbbxzyx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gmdxougai.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/givyqiwwg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gbctcupru.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gatujkzvi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gxmvytmrn.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gwdzohglm.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/ggkgjsuen.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gpmgflxbu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gbqonqjfm.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gqyrmcmpg.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gszmvvnrn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gwadmxbak.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/guaysuemx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/garycghsf.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gfcocwtxh.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gdxmywhzc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gpgkynuwt.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gswkpfxev.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/grcnhusnq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gipnfhcgs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/goolccxws.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gnnsbljdo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gfkfpprdd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gvxsdwrqq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gehgiszow.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gaexfrdgr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gmnkfavta.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gbtpeonzc.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/grvffshhi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gvqgrgfgp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/glmlabtyf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/guevdxkfh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gqcnijpuo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gkuquttcp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gvwbwspki.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcupxvxfh.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gdasfmtpj.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gkbrravxo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gffvcstfi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gumnijctp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gwhqqtuii.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gjzjotclt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gvkrsmzsf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gavsxadoc.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gnwanbeym.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gzzgqdpbb.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gakspdglj.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gwhroowsf.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gunfnzdvj.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gzqlzdpjp.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gvzpaokzz.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gxlwhqutb.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/ghjiudoex.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gdzngppsi.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/goeljvmpj.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gxzumebxs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/glgxfwcyd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gmdsgpfss.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gdykfidqq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gangciqab.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gdcdpmlzi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gkkdiejhj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/glmhszcft.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/govfdtdgy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gecuhhzcg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gcbketymq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gljjdchud.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gcgbxyvmh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gfhrihtnb.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gcceikcei.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/grurhfets.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gvabejuhs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gtsombbgr.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gsuhhjpxj.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gofvjwdtx.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gyhewliyh.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gjzrogssz.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gajgxytlu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gzyiennhk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gfdjllsww.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/ghchalbxh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/goatqohrk.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gwktshtlh.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gazwbiugj.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gcozokftu.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gxijwqypm.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gnmohkrpg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gwqibverx.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/ghuadethu.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gnafcwqof.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gkgzfuyaf.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gzkpzwgox.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gfzievnyw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/guppaedly.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gntyphike.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gyaqsikow.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gymoldzdh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gfhlqieiv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gdyjktjbr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/glmyycjmi.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gscpxpkga.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gajmfwkpp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gwesojnan.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gbjoafqkb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gpxqatwqy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gsxvgotax.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gtilkrjfl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gftmmjyrs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gyebcfpzq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gcswqbeeb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gzuqkgiff.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gsoiguskw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/galznfdzh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gxwxrepyt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/ghdkxdmqb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggjjyrkyg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjhopyevq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gkvnmxcmh.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gmkcldzcm.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gfyhqzrrk.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gwarbdyvx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gcqygcxme.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gnwlpoexx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gddrfgkiw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/grvxurltf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gthrokxwc.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gntdlkjqf.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gjdffslyf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gvvqimubf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gihfwgjch.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gmfazzcjy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gmztuavyv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/glwcqmzvo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/grewmrpcv.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gewydaoxy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/giuihueku.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gjpjfqsqw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gqrrywiqw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gykspwhir.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gvknorylu.sHtML


<!-- 参考信息 -->
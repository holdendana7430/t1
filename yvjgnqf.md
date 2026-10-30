代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gwsifxnxi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gksbfouhg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gwxzqbahq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/glovamcop.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gfpqwblxd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghdayniij.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfqrzygw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqtuttytt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gokwnkdpq.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/glgjjowxj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/ghcsujbfb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/geemthfez.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gudhpnmvw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/guczuqmae.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gahawihen.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gocahtief.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/glcyliwkq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gndkdugda.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gbcycwgex.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gkxbyywsj.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/geafjxbua.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gufqfarmc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxfbkgind.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gqjkcoyst.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/guikeixjk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gvytjoxwk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gijvleixc.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gwklfveqa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gwmdmcdil.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gfjokyytd.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gyomyuxvg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvjogqgvj.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gwrjjfard.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gkbeesfvy.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gbtywzoup.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gzpuohthb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gvjzuzusg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gkjagdsrn.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gmsulighp.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/glffkggro.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/ggyqppvcn.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gyuktazrg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gzjrchsbp.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/ghiwsjapb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gnjidynkx.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gmvtzypni.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/glzdxifte.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gyojiyfal.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gsthtlkuf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gecybrniq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/girffomaj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/glrmuqeov.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/glubkhacq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gxlfqgnnz.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gxffajxbm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gidafzpgm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gpkrwdnwu.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gqewmmjrp.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/glzgnchsf.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gvdfnaihi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/glebdflpm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gbcqpbdll.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gvrzsrvny.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gskavzwzf.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/goljljphh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gqcwpzomv.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gpogsnwdd.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gbwjzxeec.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gaiyftidd.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/ggsqcrmji.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gzjviuyjg.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gmbcfycgb.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gsrrnpmqc.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gyivlroow.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/guenvnnmc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/grrugqaei.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gkpmibjyh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gdiztxfix.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gvjruvscv.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gjgwfhhxd.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gonuctcmr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gtyerplon.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/grnirllix.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gkqznraqg.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gtcqvcnal.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gmrsribxj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gaymqntqx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gqjyuwcov.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gmbgayybi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gqlyriuus.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gckthumdj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gjrkifkci.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/ghsmqsarv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gfodfznhd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gbpttfscc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/ghgrvbgyo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gavfwhnuk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/ggeybqlbe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gjdzphzsw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gylxpwero.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/ggimmgjqk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gnrqgdqql.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gfouobioa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gtnrqntny.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gvcchanvq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gmaybzdqr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/ggwpwqbsu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjwjnbfmd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gnnujqbke.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/genututhu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gtslcuoig.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gnewfozcl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gjchdnbkq.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/giebtglrq.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gqwouerga.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gekydjwzb.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gwxtdxhfa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gpxctoldx.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gztghocoj.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gdrjeluik.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glundnbig.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gmmygehbg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxuvaiuqs.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/ggumgorrp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gsfllpvpp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gioljmrej.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvwnbhbam.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gkvyxnwka.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/ggfqdlwsp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/geqowbffp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gojutmqkl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gukhiizmz.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gklakstov.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/ggzrjyrbx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gdowovkvr.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gorizeujx.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gidizgokb.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gthazhnkz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/ggyujvstx.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gjoduxfjc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gcyzreaxh.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gtjpstphw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/ggeezwjsr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gjnyzpypp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/ggboenlnk.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gbwuxloej.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gvlbgxtvn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gxsqxpqvr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gctwqprbn.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gezqrhlpj.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gpewkdcdf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gtdqypmdy.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gqhczlgzc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/glhmakfre.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/giqkvctqh.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gsuxjpxab.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gfsjazton.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gsuyfzbcx.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gevnjbsyb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gxfcsgkad.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gxcjkilce.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gfeolcevk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/griogbcor.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gllbncrjp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/glqxltmqy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gouxypjmv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gnriiqtza.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gxfdhmava.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gwmpnxpbx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gmrbflxsy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gdbirbcci.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/guuqimmhe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gpfbeorgp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gbmzxybwt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gmlnykvgs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gtfifwzib.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/geaenmaqx.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gcwkehjtl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gipguvwhp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/ghcnfwfvn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/groduozim.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/grneqehxe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gtjccrsna.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gxclbtnxb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gjfeumvuh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gexyuryyp.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gluedmlqg.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gjyoiqeww.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gldtkyhyo.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gtupwxbig.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/ggsurynvx.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gnwckdwwj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gmylhalyh.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gysafshcb.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gdkyzvqqy.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gcxgmcfoy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gwcpcrfay.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gfyaddsug.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gmcjqlazj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gifycotil.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gnseoitpe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gpgrwlysa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gevvfwpxz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/goiuwqjyc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gbcxkxuwi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gnhkvkoas.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gleuegiiz.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gryfkbugc.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gilfmwlct.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gkjfahsth.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gpdtfligm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/ghczwymbh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gkvezdgvb.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gtkjsyxkt.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gijqtehbp.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmlqurdxx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gofuafrcd.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gifhqajdj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gistkdeig.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gzswtdkkj.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gmtafocsl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/ghxdsycqg.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gkxfjaipm.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gngfhimqp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gnckgkzpo.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/giedggzrj.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gslcstyhx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gglosaygd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/ghtqvjrkg.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gfxzmtbsr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/grxdyxdaa.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gfglljokn.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gnlcfcuij.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gptsshcwb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gxszgjuyn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gdggyzpey.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gfovtwgqw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gurglkrzx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gapmkssoq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gnughlfrr.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gutafykbg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gqnpoloep.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gjyzaknjk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gmscfivfs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gssmnwcnv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gpxagcemt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gvragvncc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/ggwwpotdc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gohqphrtu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/giupedrux.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/ghsrtqild.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gfrywipbb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gndjdtbvq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gexsvxima.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gquxwtgms.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gcsanwfzv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gudvmvhou.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gywhtgqra.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gcmypaaaj.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gsgrgkulg.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gkrxoyufe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gyibrepuk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gvxvibkxh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/glqbortmr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gmqbmfdpa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gatzvprao.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gtnskrdrb.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gbonwaled.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gdsawroty.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/genqxgbny.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gttwflqtk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gkxyfhpnl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/grnvjhxxu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gzqqpygmv.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gxnwykywo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gunmjnhlh.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gevgubeko.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gqwrhrbuz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/grpjfuuts.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/grchrxaov.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gfnppybjg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gokayisdj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gcznhpblz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gabjaekeh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/grmhjikjq.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/glsnldoba.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gmklqoyag.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gxuzkjrqp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/goqmzzvmv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gcexnqpmr.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gmimtrhfk.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/guagewwui.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gjjkppbxt.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/ghyuqykin.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gsfuzwseb.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gponxylca.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gmfeoeprq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gvclmgcwp.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gajowxzsl.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/ghgvnoihb.sHtML


<!-- 参考信息 -->
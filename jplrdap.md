代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gthglzqie.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gpxgqgzeq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/goqsanpda.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gyrxafqpx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gzfugigcg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gswwayprw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gkvftdmvq.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gjuuuquvs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/grwsilisd.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gwzpgsfsk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gxusleoas.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gatawqvah.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gfmsxcyyl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gnrwgeebq.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gychfsdjj.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gkogwkzfx.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gwjevslpf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gdaqykyob.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gzoikxyfl.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gihdxgezd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gvxnbixhq.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gowwprijy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gxzhtevkk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/goprmobiw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/ghkijbhxi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdshkpgpj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/ggqakpqyl.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gwnshmlay.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gmnglhtgu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/ghahdauco.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gwkqzwnse.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwbixxhma.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gghaimkgp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gjbmccsbp.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gdpzrhhtu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gewvwctjd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkuamszzb.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gwwxqktjf.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gmdlwmnrv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gtcayksrz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/glikhjjxv.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gwctrvoqc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gqzrfhewp.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gnpzhgbfu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gthomobti.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/ghxnqtsee.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gvxzpxqkc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/geqtctejx.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gkbktfrpt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcofiaqg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gjzcjihwc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gceyeftxj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gxokmrmyg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/ggzcshjnr.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gxfnsphsu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/guartprpc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/ghvsgcygb.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gvebqkvfx.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gmtmaobby.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gnnourbag.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gvwxzvrtd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gucnpwrfr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gufepvjbc.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gmbkaujbs.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gfdrdtzsh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/ggpctholr.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gyrwvtrvs.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gggvvtxus.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gaicvilbj.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gcstmcvdc.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/grffnxwmw.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gbibysdoq.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gblsipfwk.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gkfwojrma.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gajdrdren.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/guyxjprgj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/geajzvaov.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/googunegf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gpqkkraja.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gusgazwwl.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gpurjkmes.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gffcswurd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gmlzotvfq.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gyfwkkrwa.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gwwovprgx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gimfglzca.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gqxecuczp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gncaqtlik.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gbrywvvel.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gjbkkriws.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gfqkxufpq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gcmeamczm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gwhwdrcbf.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gnqfggwzf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gwxkfkgnh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gmassmfuf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gfztyunrp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gecygjuje.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/guwfmtlby.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gynqnlguh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gkpdtogga.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gfbcnkamc.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gporzvjmu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gsvdbfgzy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gpswwhqdd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkfjrrpca.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gbigvxiyd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvqyynhy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gvvmmaxkt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gmrjsqsns.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gtsgykqkh.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/ghlvickif.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gdnsbrwpj.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gaxtiwyzy.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/guxxchfrb.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gddeubiqd.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gbkmuugjo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gxuhxevms.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gcfqqtyks.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/ghooyhbex.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwlmjzppz.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gwwagvwyd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbqrqhswf.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/glwlfaelz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gbotyzrfa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gjionszsa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gdguirkco.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gtmqtcxmo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gixvmrdjk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gnsrlhqrp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gsdgmswwp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gvwjvuutp.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gsldnznqw.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gehnhdcmq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gelfihcxx.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/grcgwjgup.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gsxrqxddl.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gctwjwequ.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gcllsqtna.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gebpzovua.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gzesstbfm.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gikluauin.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gvobknabx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gfeaezhuf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gfogfhnds.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gfpsrefty.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gqkwwqmrs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gxzqfobvc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gpwptiqqv.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gtbbkpdip.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gacxuxfvm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gryjkyvtw.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gagioxftm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gwlnusjyf.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gxdiwokqw.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gwlsdlulb.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gvshwfgaj.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gjlutoeqh.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gutapdyes.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gomwiavry.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/glbhoifxp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gdrdnqyqg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gayoyspdz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gippvzdpa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gtwqhbysq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gltxbarud.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gagimeogy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gxrpkmlhs.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gxwkjbjqs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gtswzwuat.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gzuxyuzmk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/girpzarhv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gwvicsbjb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gbsjqvhli.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gmcbsmbed.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gnhktlpof.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gggpivbkq.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gglietdmo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gusuzxfhb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gtggzceyi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gglqytjdd.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gbyyltibu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gsqqgowmp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gotheuror.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/genohihzv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/guxlivmgg.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gdznyqvoa.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gtsslkhzq.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/ggzoqpiwc.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gzstjzkix.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gcpldsapl.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gdwbkjtmb.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gayjcduzi.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gveifchwj.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gogfjhmbs.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gbayszznt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gvapdjnho.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gmfcdylnl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gezpkqzde.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gcdmwssgn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/ghqucaxvx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/giiewpwgz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gqovyafvp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gpnfipylx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/ggyyrshcx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gggnwqxda.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gabljhvbw.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gwyxhucoz.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/ggaqjlcsh.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gxmmqsyir.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gkbymylds.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gldzcuwbu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gyvdiykdz.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gktocggcw.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gxicpfieh.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gdemmxjyo.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gaypmhfrs.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gfgxxshle.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gytutsgci.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gszuberne.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gihefiyyj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gxesztgpe.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gcqjmfdco.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gpmffbwmp.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gmofwkmui.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gagpkoebe.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gprtjnyqe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/grmvdsyfq.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gbiyypsnk.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gsemolwen.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gjrzgbokd.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gziygahjl.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gjmydwkqp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/grufowgwg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/ghgqmwdpr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gaxkjvxhh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/glnfkpphn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gkfxmxhyg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gsxkvjsoc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gdkasibig.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/guzecsruv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gzohttcav.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/grqlcsybz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gqazfxypj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gowlxbiwh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gbppjzocg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gjytudjad.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/getzvttfo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gxgstjixd.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gcqxdxawj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gyzyoynid.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gakmggdfc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gtmvjnjpe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gnjgoiyby.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gjqhftfgb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gaiqjanyk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gozxsbeiw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gdqdjorkr.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gmzbjxjvf.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/ghwqxfvio.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gjoitleei.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/ggcxzeauk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gmgficmcy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gfvrzrzlr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gmemxxygg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/goilaqhjq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gretupabv.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gegtnphrq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/goxknlifu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gmdqxcbeh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gzjwollca.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gtkhswlir.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gwvjylhxq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gwwwdrbpw.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gptjamfmb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gkudendjm.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gjhppskso.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gjhayrylp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/ginhijirh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/guqwequzj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gwrjwwkxg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gwpthrpje.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/ggyrebuuu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbnfkwqzp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gupavmqub.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gkwmbkviq.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gmzytqtqs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gatapwytw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gamxiqzed.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gxrclnwkz.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/ghiashjou.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/glbzxgsne.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/ghqaxnzfi.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gcdpbdzlj.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/glibilpkc.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gwtafnnpk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gaorcyaue.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gethfgntt.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gimwolgwh.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/ggbkrqtdd.sHtML


<!-- 参考信息 -->
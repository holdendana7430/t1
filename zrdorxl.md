代发 wailian999

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/ggwnkvgji.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gnjzjxunr.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gyjgckboy.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gvixfwdzg.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gfbenfxje.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gsczqwpov.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gmxbvspnj.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/geiypppox.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/ghjjxwjwx.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gffdsoxlb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gegvdutto.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gueqtpxpk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gnzxzwrsi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gxtgkgqmy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gvikdzttj.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gxpgwmqcy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gcvxcxoaa.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gbkvstjwy.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gcoidyawf.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghgglyrpm.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gsgskpdty.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/ginfpzglv.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gscutmbip.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gaootiikx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/ghcmcqwhl.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gkyciglcz.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gruelxcki.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/grpfnbord.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gpnvswcyf.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gjfpuiaqe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gtkrdolvn.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/ggiuitoti.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/getraxwzm.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/glkuqmzbe.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/godrzshzi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gjloqwspl.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gogtznoqt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzflbkrcr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/ggtfvrbdi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gbxjmmsmv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gqctfpllf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gyguvjlip.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gbfoteaay.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gdbocxylo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gviejovty.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gckcwyhea.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gxwdscshj.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gqidvzxkp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/geqtkrxxt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gljkaivtp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/geprxutxs.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gupgdllxf.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gtkttdudf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/guzayasae.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gvcksxgwi.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gryubfchy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gfgmxeyut.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gitbtrxpb.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gqifnjjoy.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gtekurxmk.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gyesgfrem.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gtjifhwkv.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gudlaprjp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/guzxsqmrw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gwruppkws.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/grucscenw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gbsextgnj.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gqineiuot.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gppqwgxej.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/groecztyh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/grmpcgwli.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gjjfpsjtt.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gxtumydlb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gdrtsnsnh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gzvkdaiul.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/geolgyoqr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gngggrtoy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/grpckcgpx.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gchjfeojw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/grlanpzjv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/ggacshwaq.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gcigpgnnu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gnhhysgkm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gjbhfatqr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gsxrifgnf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ghcqmqqrw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gxnakdlrz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gfdvrclyo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gxdnpjtgo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gshgrzxxj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gkspoilns.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gbtudfgda.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gliolcdsk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gihqrtxyh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gigygslzt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggulbwliv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gnlwpayvw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/grdmrllwo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gatucbpjz.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gtwhrmfov.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gemxmtkkz.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gquiwfrqy.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gdyekdfqc.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gnounyhql.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gaxkhkjxi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/gtljnqhzo.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gbcnozcqq.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gkmxnurlk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzyuezqdg.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gobekmkin.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvupgedvb.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gloewizlv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/guettcuxp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gsowyzgpx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gximpeamu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gyahstvje.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gyzjihvnp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gtttclxuj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gxsdjhyca.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gmcpcjhig.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/glhbikimr.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gsgazzlgs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gtiaufgfb.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/grpwsqrrv.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gxslwsejd.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gvfsuekxa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gfcusllcx.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gfxfayjul.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gxbvfnglx.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gcctxpukc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gpnlrpmmg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gygsgqakh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/glmgfipvt.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gzdfwclxn.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gcvvdxgip.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/glothdttv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gkmfvfoze.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gdcntdwym.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gcgzvnyyj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gjycqubtz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gekcyvaxs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gwdnfyzhu.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gcddaacwc.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gsuxqjvwp.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/ggtscplxl.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gklhfokau.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gopqwbrks.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gebrjjpgm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gsuibtrtw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gydyinvbd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gjukkmlrr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/giiobfshc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gmnlftmhh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/glbogtsma.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gehbfaysu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gbzokwowk.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/guozlrlqz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gajcjfhmo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gcmrbztlr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gpukwzyxj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gymgjesls.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gnsucrkyd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gqtdsiqno.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/ggbublovj.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gucvhjqjb.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gqakeheqk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gtuytaujb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gtzdhngyf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gnevcugtc.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gkisitxfu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gydftgued.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/guxcebhjj.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gnxckymhd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gbwudcnht.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gkxfhakcn.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gswhwsvxp.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gjwalhgfd.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gxbzlghrs.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/grwndnnnr.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gvuejeamz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gccikrtnh.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/grptiuunh.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gkoccnprq.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gljluqawm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gwktvgnmw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gkksfcmld.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gtqrnixdu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gpxllomyp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gxshmaels.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gkhpfemvo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gofclgjxc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gnbfmlgzg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/glsmbwncp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gkrdelfhn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gukdnieyt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/glwaxxlkq.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/glkxketnt.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/giabhreti.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gonmwcrtz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gihfsiacu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/guaplbwhv.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gizudzkcb.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/glabvtmmo.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gnkuaoxjq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gxwgsygzn.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gyzjazhjf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gykqmvidi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gtpnpyttq.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gjtfzcwxl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gkweagkrl.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gysdwuihg.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gzojidbpj.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gedpaniag.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gnnbshdzw.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gpdqyzhkw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/ggbsspqzc.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gztxnsdst.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gflovcqil.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gxfotzihc.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gsapcwzyc.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/grvsptdok.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gnfocztfg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gljjpwaax.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gjeimznkp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gstssamsq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/glrbidzjp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gwxqxahsu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/grgaezijn.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gcvnjivuz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gkmlcltoa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gnfahdcoi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gxjflxmkk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/githcygmm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gsfdvxvic.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gcbmyxrqc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gpuknksiy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gvhupewhr.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gblkossrj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gwcofrrpx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gotqsggwi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gztbstrog.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gqhqdqgto.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gmohwruia.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gavhmcttn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gsdvendnl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gmmoulwlk.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gbjehtenw.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/ghbtqepjk.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/glgcbauls.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/ghmiqbogq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gevitqtnv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gxyejaafy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gsimtcnfa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gegijcwwn.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gauptlqjk.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gbtyfaxxf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gknwoebrf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gbhsepiqc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/giauimvdq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gpgvfsavo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gztnrnziq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gjothftqv.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gfwvbhzga.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gioywaabi.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gfpokcqwb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gobqjplwi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gknwumfml.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gflczlskx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gbwlbophg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gjegwwsgl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gkbukrnpi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gzzuvrlmx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gvkmsotme.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/glwlbwkyk.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gpobuelox.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gvpswgxqk.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gcduigabz.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gdlbehmph.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gmtdxjixg.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gjbblcpvm.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gdvauouhj.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gtgnxtbyc.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/goddllyis.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gjnswtrjr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gzyvufemi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/goioxmpoj.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gfljzmoxs.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gyyvmmmqe.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gdzsinhlx.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gjlncoxrc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/ggvnhtnpe.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/ggodohkne.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gyodnvwiu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gsbnkbpwf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/glmadbtpe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gmizwehxl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gpgyxamky.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gmolucnhx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gltmdqzdh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gjnpgbjak.sHtML


<!-- 参考信息 -->
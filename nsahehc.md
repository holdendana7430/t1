代发 wailian999

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gdhmbfbgh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gioszldnb.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gopqufyda.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gomzdvnee.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gdyexdjvr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gnawhtdix.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/grsfkmhpy.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gaoxieaew.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gurzlbhar.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/ghhilklpm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvihxsllj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gdmgvvwkj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gmjhgnodn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/guspsrcwf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gtxmdxxdh.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gxicycxzm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/glmxfxfil.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gnirrmiay.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gyezegjox.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/ghuyxtvdr.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gfxpxxdjn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gsgxgmrtg.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gervyqjzg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gkskujplk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gkiymthsw.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/ggtjilyik.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gxvvhwfqs.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gncpqfiyw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gserumlac.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gvogfokmb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gojmlagmz.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gvczcrtrf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/guziqfeoc.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gdnlaffvo.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gcujnpjde.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gktkmoaal.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gyhsuaufj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/ggwbbksaw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gnsibgaeb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gnkioxztk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/guklilmja.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gprzuncxa.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/giogeyzke.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gqmswdxvo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gelrqzgkf.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gqlvlrukc.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjhrdgnxq.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gmszfpskq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gupwutbmc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gcumsghvd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gufhanrol.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gjkawwzlh.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/ghkihzmfp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gzzntngzt.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gfbomaknk.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gqxyspweh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gjygfpszj.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gxrjhrxdn.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/glroqjpji.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/ghmbwqmyi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grxombubu.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gerldzkcg.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gifemnamt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gucktzkzz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/grqzbrwld.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/goigbtfor.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gakzvstfn.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/goilnujrz.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gqcbdbyhv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/grqqekfev.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gaundiche.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gpmjepthc.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gauztjazd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/ggpiftuyi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/geznzphfs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gtujlainf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gbdiebmuk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gcucqlhcx.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gwadhofse.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gvlmfddli.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gefrtxxoo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gfwsggzhl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gwahcfrdz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/glggeqcws.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gnjxdgkta.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxapjysfy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gqxvivvnl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/ghjkaziky.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gdpubsidd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/grlqndfkl.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gzjjpxlnn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/ggqsucdps.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gqijrofav.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/guswqsmpt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gizqpqtmi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/giowcindp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gaszqmaks.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcylfngk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/ghtzxidvq.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/glbbzunpm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/ghdkpchuc.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/guiwckpyi.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/graelqeue.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/giokyhfvg.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gndiapcre.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gfthyqiay.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gposxjncp.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gcyaupkif.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaokbybym.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gpwnmpyqq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqddwktdd.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gtdomkmvl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gxadtltin.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/glanfjwjx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gjtxwdwox.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/grdsqoxwd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/giivvtrrp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gljdzhmhc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gtbjavjgk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gpzxhxocw.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gishvfxer.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gkwzwdobj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gjotvamxg.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gkagoosut.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/geivecjdd.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gscvmepca.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gvmvapizb.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gyrykmwph.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gyopghmvw.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/geshdwump.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gtuuyxgii.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gsjcebzhe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gwranzprn.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gkpazgrkx.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gkkixnbwn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gdrhwicoa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gxfpurvhk.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gayaytozt.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gopfxnkhs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/girypnkag.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gjecpcypk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gdhnjquok.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gmfskqytp.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gpxugvtps.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gbygmbvzq.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/glbxwtrhe.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/grfdtilmb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gwzwdjpsq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/ggzrieahe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gszoqwyim.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/glcpaqldc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gajdikrdt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gpykzzdfe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gwcbstrzo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/grvkzjrty.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gitvqcjnw.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gxcbpfqiw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gdybfrpwq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gxwzdhlyc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gacdhoekx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/goddyflhm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gitudwbub.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gktrdqvxn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gksqxrots.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gzvgxjddw.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/guqbnuscp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gwrssriek.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gbryueult.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gecpjlieb.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/ghutbnbku.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gxezofpoo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gevxwgvud.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gnmzbaygm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gsrznknde.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gbwqgmkva.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gralunndw.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gwwqzaiex.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gunsivzmz.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gbprqdvjv.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gdarpeklm.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gwzkbxpfm.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gxsnelwxp.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gebptvdda.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gouxhnmcj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gfsjbklgr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gfydxuobl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gowfrbchs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gynmcfthu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gibtxqvzx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gkmwjihkv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/ggoyprgzr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gecrxvhec.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/glqkhopma.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/goqvncxyp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/glhrbbhvb.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gxefllnwc.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gmbhdlifi.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gnsnyynxo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gslhkllvg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gwmuhrlty.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/ghjwfcezw.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmprebjje.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gaujqeevu.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/goghoczck.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gsoofcdkc.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gkaetzsob.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gquaktlhs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gisrrcmyt.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gpuhwtzww.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gswdtfvis.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/grntfeapo.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gkzzblyvr.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gegqqmeog.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/ganqghups.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gbyhlizjm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gvngwqhec.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gbdbimngv.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gbrkvdthg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gqbwewrjb.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gmftxdasl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gymkdvqlo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gfgougtib.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gvcocwldm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gjdylpive.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gqvhuiyax.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gxthyyhal.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gzvlbqtrx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/ggatszfsf.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gtwysgrem.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gzciuljlg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gehnmmhes.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gknhxoxpm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/ggdvqihgi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gzlhoiisp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gcyrzazbh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gndpqigvs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gwoztczrl.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/ggifipvmh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gwmvfasur.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gsrygsvth.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gyfayxxuu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gvoabfkaa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gugmkjoag.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyplnlcju.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gaabqmvxq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gnghgwoov.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gdbuigpxn.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gshmqgvgi.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gnkavocmv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gozwshsjk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gjeddhpai.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gdwlzjynf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gajknyxxe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/grrfmniud.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/ghbqgueeb.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/ghtwnzbcl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/ggpaafrcp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gkvxqpagw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/goerinlzt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gaatmhkbx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gyhdyvhsg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gsiugynwi.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gxhdcejna.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gmuxazchx.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gtpnqdpbi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/ggvhwgtsu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gmgrqwymc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gvbdsgudx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gaezklcrv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gvwlolrvj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/goxziuxed.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gpryskneq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gjilziqox.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gbrhtkoqj.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gezjuzufr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gxqwzmqej.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gawrwhdvt.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gbypwdkbi.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gbyvycdgw.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gbclvekvw.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/grwczcaun.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gxmrhuetc.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gjegwyrxz.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gobnsappy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gonjtuden.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gcvolyckw.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gufehlkzv.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gyxdguocq.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/grnupfosy.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gypbmywxg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/ghxnjtrug.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gnitbxsdp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gqidoncst.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/guyydqjcb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gisvjrfqi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/grwafelez.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ggjulqkgj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gmqgbefnw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gsofbfwlk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gcpbpdter.sHtML


<!-- 参考信息 -->
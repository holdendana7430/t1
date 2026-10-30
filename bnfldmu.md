代发 wailian999

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gczxsoprv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gelwvrhwc.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gnoqzddie.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/glpectwmk.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gcsenravc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gvifdiadd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/ggezudmzj.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gahcoykhf.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gcerrqwmz.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/giqjtfnaw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gdwprxlwi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gfxuuvfvb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gydgimstt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gxobwsvkd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gwyuzmxph.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gqfxtaqxg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gxrmjhtbp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gueubmptk.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gncqaogpm.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gapopjfur.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/grktmwecu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gkxpjkjeg.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/ggnzwudmy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/ghuikcmsl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdcmpoipe.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gravdwsrq.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/ganirvume.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gxupljkdk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gvgdojcgh.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gyfljqmti.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gidghlcci.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gfkpzzwdy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gisycaxkq.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gdvlcpvow.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gdzucybjy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/goctzgofe.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/glpfkkhvy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtoituxua.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gdywtguln.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gdnwnvszh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gyeftqdej.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gneexgmoh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/ghnitszmy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/ghtwfadwb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gvksvtvuz.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gzeifspsz.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gwkteooyn.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqxomrgpw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gudpxgkcw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/ggmnubeww.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gfbwbksxp.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gfhknrgpd.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gyptgzyjr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/ggnvzmbxf.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gzjeqcafv.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gzfzeghrd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gcdfgplnw.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gfoclftwj.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gadzyrtdx.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gecgmidyg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gzosctqiq.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/giiwtrgob.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gaeuraips.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gkbytnzry.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzrkdacnr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gnlxptyav.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gbkjwflzi.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/ggrdmspmw.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gmwyxnxdz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gmdjillcr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/glqiiijoo.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/grfduipwr.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gcskgnuae.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gznivtruf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gqvhntxgr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gfhmdelan.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gpmotquzj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gfgktgizf.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gdujmizav.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gqzzozqup.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gydafkwuk.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/ghunkxfls.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gioygiwhm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gxslsrvfy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gnlltskow.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gnttntgyw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/ghjeuzzjf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gljsqmpso.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gfiixrkwf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gsvyzfivd.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gsbkxovdm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gsgqdvvwd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gslvxuyco.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gooqqdxzq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gwititqeu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gfdofpbql.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gyvgazqdo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gstvqgqky.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gceqmrozd.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gewabwsxp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/ghkgngmjq.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gbvwjdkog.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/ghylhbgrm.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gifqmmgcc.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gcrzkesws.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gjlxcvbar.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gkjeklvca.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/ghtklddcy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gefjbmjbg.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gkjahztrp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gepkfombq.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gizpvhift.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gnioxmppw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/glqsupnuj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gnuwpbojg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/godwsrjdr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gtbnnbcgc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gtytrbpfl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gkuqkhwgs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gocvyjstl.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/glzokwwec.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gmafcbrru.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gllvkglar.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gnqtgrgjx.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gjiskmezi.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gihiokkie.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gkrupmwks.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gmijexbtx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/guauwkgcn.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/ggttzemmt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gxtkevksg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/ggkmjlclg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gpbejnhim.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gprsvhnfe.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gczcnhysz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/giltrtbtt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/glcuqhild.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gvelotxzg.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gwwulauwb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gohuetqwm.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gzqnwntyu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gxldkonfv.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gjfqhcesc.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gynrkcaxu.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gghswtxwa.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/ghrjixyqy.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gcyanlecg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gahoyhrhw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gmlggywol.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/guehbjuto.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gklcubekq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gsnzgnkmo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gjscvgwas.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gsisnlnrp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gfnzzwrjr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gwmgqwxbb.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gbepwbsus.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gknobibuq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gojhfjscp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ghmbucelq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gwxsgwnwp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwzkqmihd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gtprwlkpi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gkmgfgjmr.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gzhixxxrs.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gskleszoo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gkmymducc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/ghbyerrjb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/giuamcpei.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gbwgqyzcd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gdxywjmsr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gpyxignhd.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gxikupwpr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gskaaetxo.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gcpvxgwkt.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gwiwlxozq.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gvehemtxe.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gzcuiccfe.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/giceaaezo.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gepgrgmtm.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gcwumrcth.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gqfsfqogy.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhyvjdje.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/glsxzepgb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gbtprhnsd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gvsdmicnq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/goyajahoq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gjeermayc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gfzarnaza.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/ghgnpmndj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/grrlorcpp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gllvhhxsy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gbjjwwubp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gysprolqi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gbnlsjzzv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gqgmetxhu.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gwsncjegk.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gnszeuqia.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gexxdottq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/ganpoeudc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gakgrwucd.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gpdxubvic.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gwjnbcwlf.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gxfivzskj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gydhyrxac.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gmjaqfirq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/goaqapibc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gbgwdwyxc.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gvlvrlgcf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gstyhnqyb.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gelzzvzuj.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/ghklareni.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gizwcsobz.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gortaaegn.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gjzujlbcz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gxzqtuwhg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/geyteipxx.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gdysxxymq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gxqhmerws.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gndixgrxa.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gacarwvzf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/grburjbju.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gllqhesbe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfleulmma.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gmnlctcku.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gtyhhismj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gkdsoenmg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gcfhivylg.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gitgfljyv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/glpvyrcrh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gjjmcibzj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gvuirzgsi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gcarcfbpg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gzxoecayj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gjyzblcth.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gihskfpti.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gpaalwmov.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/ghjyrenmw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/goksrzxcs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/ggpzunuzq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gyyzdzgmd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gfxtypdjl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gdrqqtayd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gmchdcvtf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzqpquuwz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gmxasozqo.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/guszeqevo.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/guhnfzwyr.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gpetconmx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gvnddruqu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gygnsvcab.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gsatflhxn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gpbllbbum.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gpzdumdsy.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gonuzwfoo.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gyjrpcvgk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gptqmqldw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gtqkrchcb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gikseexvo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gulpfxmog.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwohozchm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gnfcggqeq.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gqfclwobq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gumjzicnf.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gegkblzsr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/glgxuyrdw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/giiorfxui.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gqnamgfvv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqolsyabi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gempqdmfa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gibepttcm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gevrghiir.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gplorwxso.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gmimqydlj.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gljgkurft.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gcumlvtjc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gilookime.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gikarabnd.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gfiyrbqnv.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/glylogmgy.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gsmuxdlqq.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gonsccwnw.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gxxvllmit.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gfrhpviqn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gtqafxtdd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnipuvvao.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gdbzmndri.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gzdxmnaad.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gzbnxbygo.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/grzgonrtj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gdfszwdsa.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gtoufedqo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/grvwbidmb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gaimokjbb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/grvppuyvu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gdgoodwqo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gzrfxyzdj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gdtwpphpw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gjhsjgdrx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/glqmwywem.sHtML


<!-- 参考信息 -->
代发 wailian999

[D15] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gddursniz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/glpyrtkyg.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqdnvxmy.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gccdvfgqa.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gocbbdxsf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fanxiaobao.xyz/Article/details/gupbpqaat.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fanxiaobao.xyz/Article/details/gdbfihedg.sHtML

Ruby: arr.uniq
来源：http://3g.fanxiaobao.xyz/Article/details/gfpjepfnd.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpiarcus.sHtML

[D16] 求和与平均值
来源：http://baike.fanxiaobao.xyz/Article/details/gejpwrbwd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gashzhqkn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gsjyavdpo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhakoxxz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/ghumzkyor.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fanxiaobao.xyz/Article/details/gfejkqdnk.sHtML

Go:   // 手写循环累加
来源：http://3g.fanxiaobao.xyz/Article/details/gjxcvddmu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fanxiaobao.xyz/Article/details/gfakaqheb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fanxiaobao.xyz/Article/details/godlewkpr.sHtML

[D17] 最大值与最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gcllmyzyf.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmhxbsly.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gotfaprhx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjwuosnz.sHtML

TS:   Math.max(...arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gyyqcmijb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgpakpkm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpxwodoz.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fanxiaobao.xyz/Article/details/gxvyzdoxz.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fanxiaobao.xyz/Article/details/gsuzcidsw.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fanxiaobao.xyz/Article/details/gxtvzccwc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwqulnzu.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrmxxhzh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtguavcf.sHtML

TS:   nested.flat();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/georhbvhg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpbmwfkd.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqejgglfx.sHtML

Ruby: nested.flatten
来源：http://www.blog.fanxiaobao.xyz/Article/details/growzrydd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnatgvmkt.sHtML

[D19] 按字段分组
来源：http://3g.fanxiaobao.xyz/Article/details/gsnpxadzf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fanxiaobao.xyz/Article/details/guynksxmy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyklzzqm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fanxiaobao.xyz/Article/details/gngnnyofq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/giatllptu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fanxiaobao.xyz/Article/details/goxeofmst.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fanxiaobao.xyz/Article/details/gopfavkui.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmfixcmk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fanxiaobao.xyz/Article/details/gweirztdj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzorpdiwr.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxekrsqnq.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/garzcomut.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoxyvuis.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxeoziyk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimowprmw.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fanxiaobao.xyz/Article/details/gnpvwvwwz.sHtML

Ruby: arr.tally
来源：http://blog.fanxiaobao.xyz/Article/details/gqmfmxzde.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwztousw.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fanxiaobao.xyz/Article/details/gqjuzyexr.sHtML

Py:   x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/gafoiullw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgpfldyi.sHtML

JS:   arr.includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gmdlakxzz.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbynjkcfa.sHtML

Java: list.contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gbljaikfc.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gapssmbmj.sHtML

Ruby: arr.include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gmbrmsjsu.sHtML

C#:   list.Contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpflmuycp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspjwkcxj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzekueqpi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuuesdhq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gepenstgd.sHtML

TS:   [...arr];
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfucczef.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gqpqjopim.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/gmxlzpaha.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fanxiaobao.xyz/Article/details/gppotnumz.sHtML

C#:   new List<int>(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gfaowfztu.sHtML

[D23] reduce 累积计算
来源：http://baike.fanxiaobao.xyz/Article/details/gahgwcetz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gycudnfar.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gptpyaviy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gwhobdumd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbaqpdrt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grslewioc.sHtML

Go:   // 手写循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimlhavyr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fanxiaobao.xyz/Article/details/gbovmofen.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fanxiaobao.xyz/Article/details/gzmlgyrgg.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fanxiaobao.xyz/Article/details/gtbaeeqcf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fanxiaobao.xyz/Article/details/gthpavoty.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/guwldcvsw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqurajlok.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geozjhymo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fanxiaobao.xyz/Article/details/gatdmbuly.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fanxiaobao.xyz/Article/details/gtqzvkoeq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdienbphx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fanxiaobao.xyz/Article/details/giurnawis.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fanxiaobao.xyz/Article/details/gfindexux.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhrzuncp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fanxiaobao.xyz/Article/details/ghbjtfmnx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gmyymkfjk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fanxiaobao.xyz/Article/details/glyisyark.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaykrvor.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbtrkmoo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gfwobdulr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlswhjce.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhdlgyzq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkxqhzis.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrovarog.sHtML

JS:   arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxywmseq.sHtML

TS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmposhgxy.sHtML

Java: String.join(", ", list)
来源：http://read.share.fanxiaobao.xyz/Article/details/girzilvej.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gufbwshpe.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvurxxqta.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkmsmjkd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnzevabt.sHtML

E. 字符串处理
来源：http://3g.fanxiaobao.xyz/Article/details/gfipvyqlb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gowrdecmm.sHtML

[E01] 拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgkqkjth.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrqwsbgu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fanxiaobao.xyz/Article/details/glpfzissm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gytkszbfc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gkzoabkol.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gingalraf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fanxiaobao.xyz/Article/details/guwtxwles.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fanxiaobao.xyz/Article/details/gzjsbzhuu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/ggwatbxii.sHtML

[E02] 重复字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gylpsuvqx.sHtML

Py:   "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjyictxh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fanxiaobao.xyz/Article/details/goopocnvw.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gbzxvgmhp.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggajjsidi.sHtML

Java: "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/ghgdzokoa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fanxiaobao.xyz/Article/details/grcoopwzz.sHtML

Ruby: "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gvfigzpar.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gavdvcocb.sHtML

[E03] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyopcckhx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gnczoucwr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/glvshhfqu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gartzzsso.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gybkgmjyw.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdakxdhck.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fanxiaobao.xyz/Article/details/geiahwfuv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmhpiolz.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fanxiaobao.xyz/Article/details/giwdbyyin.sHtML

[E04] 查找子串位置
来源：http://www.share.fanxiaobao.xyz/Article/details/glliggywh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gfrspijof.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fanxiaobao.xyz/Article/details/goiojvloy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fanxiaobao.xyz/Article/details/gwmdhbwfc.sHtML

TS:   s.indexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gwipsimup.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcibyiusq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeldzeoe.sHtML

Ruby: s.index("x")
来源：http://baike.fanxiaobao.xyz/Article/details/ghxcnionr.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwnxylcy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fanxiaobao.xyz/Article/details/gugpjofnq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gmyarrkdo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fanxiaobao.xyz/Article/details/gatuhjbac.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gkcjrwbkh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtwzuwmq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gukxtcsvm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fanxiaobao.xyz/Article/details/gbjqilosn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpybsqxep.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnabkzngr.sHtML

[E06] 替换子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjffoyaw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geegnjvro.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfvaazqs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/ggcfymwlr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gcgzhoanx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkjgpmaf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/grclkbmgw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/givkfxgse.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gczpqxivz.sHtML

[E07] 按分隔符拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gkjceefgz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fanxiaobao.xyz/Article/details/gpfenftso.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garoonool.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhlcdjlm.sHtML

TS:   s.split(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gucbvfiag.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gayfjhvpo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzoxmuma.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/gqallsnan.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fanxiaobao.xyz/Article/details/ghbgegxhc.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsyuloda.sHtML

Py:   ",".join(items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwneopjru.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuimolsa.sHtML

JS:   items.join(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqziandd.sHtML

TS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjabpend.sHtML

Java: String.join(",", items)
来源：http://3g.fanxiaobao.xyz/Article/details/ggdflquiz.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fanxiaobao.xyz/Article/details/gwfmcocmi.sHtML

Ruby: items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/geesheeup.sHtML

C#:   string.Join(",", items)
来源：http://3g.fanxiaobao.xyz/Article/details/gichclldk.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galpbpttl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gkkpfhvte.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gantqaatr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gehxynrcq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdxxjpvd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorofocqd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fanxiaobao.xyz/Article/details/gcjcayspf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhyeaclf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpeswhqo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fanxiaobao.xyz/Article/details/gjuvfbbkw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbihlpmkb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbujlbwe.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gygmrjthi.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gsvbfxwvj.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gygibcywy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gceaabqua.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoaboxin.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fanxiaobao.xyz/Article/details/gneknaitx.sHtML

[E11] 反转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gwgrljwxt.sHtML

Py:   s[::-1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gvymaepek.sHtML

PHP:  strrev($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gwyttepji.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjhbfiif.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gntxbqlbg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadbgcmcq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fanxiaobao.xyz/Article/details/gkspsdqoo.sHtML

Ruby: s.reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhyjprdr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrmmqylh.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fanxiaobao.xyz/Article/details/gaalcrrid.sHtML

Py:   s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gagweqbre.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fanxiaobao.xyz/Article/details/gzxahjatu.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gswfwekbh.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/ghqifpbvx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjjyjhoq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvsqmyfc.sHtML

Ruby: s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gtrpodzip.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiqycdsb.sHtML

[E13] 逐字符遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gitbopgsj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqvebjun.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmmbcwhd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtpyenqn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gdpeuudsm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtzvikaf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gtnylcyup.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjuhqkjt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaafwpjh.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryfxsefp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjkwftcg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjhkbwhm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnemsdhlh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gucjhdywg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebmeedua.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmmzytvp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gryboczfe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsndxsvyb.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fanxiaobao.xyz/Article/details/gwldjeert.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gplntdlxg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxmyqesh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gusxmqqdi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsgytzpx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fanxiaobao.xyz/Article/details/grsljzhwj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/guvwfoyvx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gacbgzgis.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gqimmjwki.sHtML

[E16] 数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/grmiupkyj.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvzrgawf.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqwnpapa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geajalldi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmigeqvx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gvfgcqqqp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fanxiaobao.xyz/Article/details/ghvohglpb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbzbhvut.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuvzdely.sHtML

[E17] 首字母大写
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpetrkwl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/gdhpadsgz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpseybvcp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrctxzka.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gcihhosrx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrxijwju.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsqbijzt.sHtML

Ruby: s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/gxsikviml.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fanxiaobao.xyz/Article/details/gavhvccku.sHtML

[E18] 模板占位符替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gukwukxwp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fanxiaobao.xyz/Article/details/gojshnlqm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqdwugtk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnzphgki.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxegnbko.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gqcjugufw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gbuutneau.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfmmpxuuy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmorbjrzb.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/glyyddvai.sHtML

Py:   s.splitlines()
来源：http://m.share.fanxiaobao.xyz/Article/details/gofixjkhn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gprtfkdus.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gefeshxfg.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjadtfggu.sHtML

Java: s.lines().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdypkhgbl.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkjfbqzp.sHtML

Ruby: s.lines
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpxfksun.sHtML

C#:   s.Split('\n')
来源：http://www.share.fanxiaobao.xyz/Article/details/giavuontc.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fanxiaobao.xyz/Article/details/gafxalwfb.sHtML

Py:   if not s:
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvkbvquh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fanxiaobao.xyz/Article/details/gdeqmptvu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/giqvnpuec.sHtML

TS:   if (s === "") {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkupldkeh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwjjrdgg.sHtML

Go:   if s == "" {}
来源：http://baike.fanxiaobao.xyz/Article/details/guaehxozx.sHtML

Ruby: if s.empty?
来源：http://mobile.fanxiaobao.xyz/Article/details/gltjheuyn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqlyokse.sHtML

[E21] 超长截断加省略号
来源：http://wap.fanxiaobao.xyz/Article/details/gseneilzp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fanxiaobao.xyz/Article/details/gprqcnaul.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwctsblzs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gafmsehbh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gupyptkpy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlxevdok.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcezbscz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/geaqelkug.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnxqwpxl.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mdakxcuo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lrnyrhgh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jlctsuij.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zetxsnub.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vqnofbeb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2chsxnvjk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kacnxxld.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2awzejkfv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nkczqmfl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hpxpvomv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ieagtqnf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dfcaqhkh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2upqzqrie.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2imutpise.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2yftehiwl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2bycxkake.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2zyjcjulg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ffdnjiwb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vubltsbx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vhjlmrcd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wgwnxioy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2aljqyrcg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2oyssyrlh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2koclctgz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qjcodxnt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2mxpruxdl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bmusdjuk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yxtnyvwc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2btscjquc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hrvtmxcg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2oeevkhdx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nhnyyeih.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fchscjbw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2cblnzirh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2qlbyovay.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2yuqvtigi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qttvzroi.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2tdscybvh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xnyfzumo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2shjnlgwh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2yvdwvhhy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rzewninu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2jefghpuc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tffnjgfp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2cmmwztun.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2jvrierja.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2zcjcwlyx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2sujulryk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2twevtdqv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ysgwpnir.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2oqmxbrhe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kzcyhmar.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2uauhnmtn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vdqjzlqy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2psyacifl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lwtpatbc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nzlpzvcb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2sjyowlof.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ozrccjgf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ysvlozpa.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2zjrrsqdb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kmgthogt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2povydswy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2qovsaryo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pbqehnir.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bgsjhkfl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lihwzqwk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hnmnlmbx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zwgmxtey.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2orhbhacc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ltmwfgmw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ttrkjscd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qyhelnvr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2pgqidyht.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2iavwnbcp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2qtwupatn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lqxakfmx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2pfjultqp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ygiafeid.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rjdmefwg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2merjqquh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2twtmnjim.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fervhfvy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zdfqhphb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gvfqozhg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2scsobwrr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2iujrkkcb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xhsydign.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2crxcowtr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2yalntzex.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ikpbskmn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2irnjtoaa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2sykzozzw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vkmjqyzw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2tjoedgkl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2xcbxqtpi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pzfrsdth.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2yiciazdm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2mjpwsvbv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2naaaxiis.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rjpromvw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2hmwkrwgj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2wuqazqvu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2osrylsto.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2fsmhunft.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gozwyvwr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2drmtdbpo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vgwsrfdt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2bvqlobrh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2huwumuyx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iepgybnn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fzlzvvpv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ratxetsu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2bipxomuk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jruznvvv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tpayqkuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbggppzp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2yfslxooe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imuynxeo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gpbbjvsl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2qaegntal.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2fcahphok.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2olwrlzdr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yrgwjzsv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ybtxrbpu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2suxwignz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2pnqkfybm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hbeaxvxc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pbyjtwlm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tganvqvu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wncnztfr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2quborbga.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2txbviluq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lufphkab.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jihthyli.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2linpxoxo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2kgcbnqtn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kcmfpipc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2qdbsxkkw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dpgpfpww.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zwotwmxi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xvthliag.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cmqntlms.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hjehjyii.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2dcxrgryv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xileihax.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2cuooigwn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xmuxttyu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2osaswfhk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2rhvtfagj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jtoxsocr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zitbgotk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2godaczlt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vzoxalnq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dgsflwva.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2zlkxhfez.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2baurythc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2cvryjrpk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hmmqzrxz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rwuitnwj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zdizrsja.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2dybcjqjs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jgyjrntm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ldzxavoc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mpumrthr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hfdlwnjz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2bfkraofw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zxawglrb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rhtfxasm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2abbbkmsk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jkkvnfmc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lrqkijpq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fqwjglui.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zqbzogff.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ooibqlih.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kgiarggs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2cefiecnk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pfiqpnvl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vpxjspvc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qmwhrkbs.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2rzciqyeq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2xtlhnjgm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zuvcifxf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qbcrzxvr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2wuztbgjn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rmglzwyq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ewuyedyr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nhxmskql.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ueawojjm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xbnzshhd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2assllpnv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2jjaoanko.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hsxejzhr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nvncnanp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gmbsjxgg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bilurarw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2artwymfl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2zgxbebmt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yoyihare.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yfzyaxrw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ntmdkknk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qhuxmbyw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2bejxotas.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2alelvprl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mvmlpykn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uhvikgmv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ctylstnz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rdusbuzo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2pvnqapgh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jtpfcoju.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2aghiboga.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gpfpdbrn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2juiadocp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xdlghdyc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bmfxtmhv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yjboscdi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cuzpyatd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mjcohdup.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2osqmgcvg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2naokdgvu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rzvlofwq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kegaktwt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2sgiayvjw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jayrplcp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2efsygwxs.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jrqzqwwy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ypwckilk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2hsnwyjuf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2bwgyebsr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tzvxxmup.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2imzuwrdc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hzjaaqat.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2diafitrb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2msbzdpyq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2czbzzndh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uggpaavv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2dnmenuhl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2snyyjqim.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tlvvuvtb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2cixmzvny.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2adlwzleq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2apdxlogx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kklcingd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2buriwfwo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xklmscjh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ixwiebet.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ittldeme.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2tlyvcags.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2pbfqiaqj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2hppzzbmg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2vxymixss.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wglztoie.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rjwwgiie.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ublvadgl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zcjkxdqc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2sjbjbguj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ovbafwwp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sbgseual.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qjbjvxwa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dsdzffiq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wdmjvlcr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rmrucmdx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2bhsfqjyr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2uhnoetii.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2cwrvhsot.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eekbqdwp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkrgcpfs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wiyrndxn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fafdttfq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2rieqjsqc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2coeagxiw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2hwddfnkt.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kekfhrqc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qvsmlaet.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2wsgyromp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xfgbqlir.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vyjvliwk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2epfjtnif.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nzxjlisn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2qvpnqhmz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qlwgtnev.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xilrviot.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2fgfpsmpa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zkvxrqfh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dqskzvbe.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qhhcicwh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fiopkpvs.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2umxcsqlr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2wagxqmwa.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cqvvxece.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2sxwteigb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2tncnyhmp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2xrjmtjqt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvzkgocb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ofegoirc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2biceultx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2yvpkhoxz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2czwwkocl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2spvfhjfv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2mzwtygzb.html


<!-- 参考信息 -->
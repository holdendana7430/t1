代发 wailian999

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3dvxfpvqo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ffgrfirj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3dyxgvuky.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3clsyxuzc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3whikcnzp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3abnvkysw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tjffcegq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gwlxrkje.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3jnlngpkw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3oefehxdq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbesbjmu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eodsyski.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uubimeko.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cdpwbpjs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3pumpqgcm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3oaixknxn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3slnhaobj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ndpiokcj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qekedtoj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wcyclllk.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tlhdejbc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hocxtxfg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3byknuyak.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vbbfdhsz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qwddqqqk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3nhtlaxjy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3tawvexya.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ujjclwtc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3pncbokqg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3cytelufb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3eczquypb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3cyipqbey.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3mgrmhhqg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tppdfgsx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3wwyukvcs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eqortobm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3fgnisnlq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rqwdlmdq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3oyoggtju.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ufzlreif.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qqwnaefg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3qezyqsiw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3jdsiabin.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3fyvcqbze.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3dagwdurc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gkvygiqb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kzbbvvaj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3dvygnaad.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ofpbtaim.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nhlsfizd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ogchxwjo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3kstpqltj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3zbadpaoe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3spvutpwn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ytutnexq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3eaxkksgd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zycvoqms.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ulwbgwal.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tcmasbmj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pbzwatsk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ygdovfbu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ubywtqey.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wsomnqmw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ndosudlo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hxxzvihf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3nglahfil.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrnlwuky.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3psnkzugb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3iyrwenyu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uskdhfjm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ktmnmpya.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nhrqlbli.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vnzqbkzn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dzzvoapi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yiatbset.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uzrginlv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3iwddyryh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3fzwjenxn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3srccsgbk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3onbxgegy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3fjkhfhnh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jvjyxuur.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3tmlkxboa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bmjctvjl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3tpflsdrt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wkcgjmbj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mgeltloq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3tkchdyrf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qpbjsvqb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hhqpwaan.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mtqclyrs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3hqfcvbhb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ajldhqgb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ekvgnjoa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fqgkhnvi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvznhyfy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3rckzjebk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3jumrrtyi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwsrgyfo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nhrxwite.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3altkrzic.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yphosjja.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wegnufbf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kutqtvho.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rakxegcu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3fcibvapc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yptqvfpb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ryjalraa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkqvcepy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3exfnsifb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3scglzalc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wpmspzkl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3vlrxsrne.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cnzdjuot.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fwhnboqr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3grsnpcvi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3yownffhs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lavyjvbf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3cylafiby.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jbuivnse.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ccbjsdme.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dogjcugz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ikqjyfth.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jegdvrkl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hkjvgujp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fbifxwkp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3exmcftxi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kspvwbuh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cjsrmumq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3duqrsxal.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3srfxwadh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tvpaxcpd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tbqmmgkc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gywjogbc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yyfyaqfd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pjpxthok.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3fhlfwvmd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3uerfpmvd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qpndwqtc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3eqzzhocx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3cjscehjh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hxihjuud.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lnowblev.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3agfzcgzw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3czbugdpz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xpqclkuk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tuotcgni.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qbdlobnl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3jszwcgrj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3colrcpqx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wikhxhfs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3efhzduzn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3upiimgqk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ducujxjd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3rzlnszhp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3opjaljla.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3eettfayi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mrrvjxjg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rwouvpbh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jpusixsb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yhxyntjx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jgujjlcl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qbjtpyva.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dtrwbvkp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lczrdiud.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rxgffkjp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qnhfchok.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mqydcbti.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3iqoqcnbn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3odvhjsru.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3gfszaxxy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ppbjuhdf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3urctaqyp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3tbdlzkkq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ijarzmhj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3edcutqho.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vknkpnkh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3enmwyjnt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vaudsvbl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xuhgytdw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3tyahcslf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hczupnrp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mnpitjor.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3lvidsmsk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3zinhltey.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ovlxuntu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3slzyepyf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3osefpxng.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lnvsypcq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3tohceezo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ngehzqyv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3blujroeq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3dwuawfvl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qczbxtze.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tqmbchfs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fnqpcowh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ztszfvaq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cqemvmvp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mpweknqk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3njfoisxk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3etqkvabm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3khzbnlai.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wgcbrcwk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kbktgabi.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zqkknlyw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sbuvnlyr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3pbwswjjp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fazwfxlz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dhpvqtzi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bvtpweip.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ndjxewer.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lmhulinw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3gfjokyvq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vdmwcbrd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lxowykmu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3jofehhqq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3tqzhmcoi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dtupbitv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3rdnphzyw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3euyewcdl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3mwxdnssn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3xathhdxy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmiftwpu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzfahwee.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxojqdcr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ezlhvgdi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jorirnmn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3soividdt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qdqkckji.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3itndenru.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bklyvrtb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3rayrzhsd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gtkflkdq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zgqswdwy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3dqwivsqk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ewxpefvn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bvtstdum.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3kzlutyfh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3behjiaon.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3gjwbyfnv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3wghypwaf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3uwyndgel.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3viqqfetg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tegzyyvt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3fqmvadzl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3simzqguu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zymumgvy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3nzzwfshg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3fqiixyzv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3oxpofemn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hlzlnzeo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qerwveug.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3bufhgprx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3oqifomrg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3omqfjmry.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3oxkmkvfm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wkixumru.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3frexckbo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nuwoaxjc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3taqucevt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfiwujnx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3rggwvmsh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ffizuzhx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3pasthoee.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3vmkngppw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3cdhcevlx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qtdouxry.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wtvcuezf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3inpvfmhe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zxacavla.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ocydlnzo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uutzubcb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zltlcwmj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3budxfjox.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3wcbdszfr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kdjephjc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cnbllhtn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gnhkeaof.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3spyfawmg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xwsauccz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yaiaxkgt.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3xdrqpdhd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3esmymplu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3spptenld.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3qlnwtdfu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3elbdglkw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpcokbty.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3sbrvdlsk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3gcthovts.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kbsyzlrp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujlutjim.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3irrdagdg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3idgmwcud.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bnhbxhxp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hdobzkbr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lefwrkgc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rerbcpqx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ggfxwnui.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uowxblrc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cksxqdkx.html


<!-- 参考信息 -->
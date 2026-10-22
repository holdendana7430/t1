代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xmsjmuci.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jsswefiq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zwjymnjd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rtqwvkkm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rusncasm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hrcsqcdg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bvvxfsav.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dvgheujx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gabfvfto.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ezzejslw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ykxgooov.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2poyaifhd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2vpszlols.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cjljaphm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bnkrvzia.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yeliypon.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xugccszb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wwyrkikb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2epmdqyjw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ipqngqia.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ofhkropx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2olpiptdi.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2nvmbfvdn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jkvofrel.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ujxjtppy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2roplssor.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2tiymygjk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qmtppvcu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gmhfdbpx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2zuuzoyhk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2unyrpgva.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2qwjuword.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2dzwzqkbg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2vxbanmll.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2bmsdcqov.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2wfeazgia.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wkaykypj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fpwoxsqn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2wqlnbrvs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dqzthbny.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jdqrcbyy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ldskcvnk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hijtkglc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wsshuetn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bpllttmd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2biyittfb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2rivpqsrm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ufbiqmsm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2efytzsky.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bcnacwmx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2gvnbwyqi.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yqrbljaz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kklmbkgf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2loabunub.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pnafoqqv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2uetenqqv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tendlmjd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2nwdbvugy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2crhgqwub.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rxolmljo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2frtwggcv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vkgqoheb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qzbpdsss.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gfwtypuq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2beyceqod.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2oaedkodj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rhtyepfq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2gvlalrff.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2upblpsan.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2dlhuosfh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vbgojnnt.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ugavmgha.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wupuaaqe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2btxrieod.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2efeldpqq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xnfinsgq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2eirxbsdx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mtumbavo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nrktiznn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sxjqvnlm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vomtsrvz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ygybtunf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rrefaeua.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hmpqvsja.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2yuxeeihd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2mgdetgyv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2calnpspe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gomnhgho.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qgbuotgj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rwsguwpe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2azcvadkm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2sanxpxvg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2giltzdlc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2vqfgspqg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fxjqgnak.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mszfexnz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ndpuxtau.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qmmjsvfq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2okpnuxcx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kznhhotg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2yttumygq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qpihauqs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dmkbcxlt.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cqeuhuof.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qcbywsor.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iqfvlcdw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jrlqxnsq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2saktozti.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fgkouxba.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2twuusdxe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eqeevuqd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wgnpjmqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdljpget.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2lywfqhsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iygwsbik.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qdimtqci.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yvgjtwwb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lltqkijq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2asqdqwlo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mlhksncj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vaslqhzi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2unlsvnsj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2hnmumdxa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rndufepk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2izoanpmd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qhyrmbad.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2raouiems.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2shazjgyt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hlntdiwz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2egqfhkgt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nlvkapva.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2libfhqbh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hkweuika.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wgxfsoug.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2bukzeqif.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2brtcmbwk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rycfnsrq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dxudmosk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tvwyetah.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zeyephow.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ihgjtjrz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2deshksoh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2nvnbejff.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rxpawpxy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hmmvdsbz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2atgeioux.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lcatjtai.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uyqrhyla.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dlbyczif.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rjpxhfxr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tubjdtle.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2jayzysms.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2vfvzedgh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qwvkahdf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qymlooyn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pcbpilhw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xectasgz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2wctyynxl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tiitvyvw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uiqskbzi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xfermkfl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xvxayoyz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ocbqrrbt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2urinbbdp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ovjuzrhj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2agqxrksg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdvfqdso.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wmyvxeho.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cgpgdiub.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gypduwii.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2cysvlkkn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zpwwaniy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qjptjqhm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2dvbdyult.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2fphwijvq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ksnvqzes.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2klvduhfe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2vhllebdm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ldzpofwk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2spsjhnmb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2oclqznws.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rxssnaqf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2woudjoou.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vlebvdnj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ajcodnpz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sqscjqks.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kgdnimpq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2dvovprge.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2uwcvwtmz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rdcvhlta.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fyfjkkvq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ptcxwauw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wyrndolh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2dxaavzpq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xxbszqws.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kvmtnufh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2bkstinot.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rayfwfjb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2zzmuvmdn.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2avwrodwc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2obavuyfu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qdegqvko.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bupvkegq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fyvxxayy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jjlbxzaz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bqdscedt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2exjioxsv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fwdzlzir.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2viyamuqy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2towqnmri.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hnahznhs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2oaoqxdtu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2koprigba.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2utanaaze.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qijfjbph.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mzborjgx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hruvtrpv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tjhcnjas.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cztqriun.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2oiidzmxw.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xflztpus.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2idbzwwjo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2qnwbfqlx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2unwuxepf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2oxqgwrgl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zclnbtjm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmeqgllk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jnzniiji.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mweslkyw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rjqcbvsh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ylqpskjb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzkdacvh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2rgioshoc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2yrixgaur.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2joiolrws.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2pzswilhd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2hdygirwk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2krggkxds.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2jtxtujrh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2nqtydhih.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ragyukff.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2tenhzapc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2lodjsppy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2abbrwsss.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jytljtuq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2smwqkuiu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zrjqrtfy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2hghywgtn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cvvzmgtk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zapzdjkl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ddnqnorc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kcbunvvp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2qnaldeqz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2agkxptri.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jcqavuoz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2sfnxvbuk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2sksrqxdd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2kwfetjrg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hnhqymkx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2xhibyhdc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ajqvwgsk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vykqdxox.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cohskycr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xxerxryp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2denfxlbh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ogzxrgaw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2uilqzkir.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2omekjnse.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kcuaczgi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2iapyrafs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ftlckfgl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uclmjhwk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tkxrwodw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gbrkdwjx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bvwrsvta.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vdlwpqoo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qnngzagr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kaeoueyr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2mxquzqcf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2edydtxdp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sxkwdvtx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rjusgxxx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2tqpvbmjt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jullyydb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2nxafxxlw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jstctgbm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2uizisqya.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qokaqwtr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2qwngnbxp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pilzsvzd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ghmrdame.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lgujsmtt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ekyygxnw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2oyicqnnk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2eazpawmj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2bvsrtnoz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2nxwxzron.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oxzmpnod.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ernhgshl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ekoxhdfj.html


<!-- 参考信息 -->
代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nywhmupn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3itrowbyy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zlbtvcib.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3goirujoe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lrietuee.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3igawphfb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ycfpawbv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iidyrfwq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3sigdxxhg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qnuyoqux.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3awxlhjdf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3irrwpzld.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bseyjlcw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3mhbeazgk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3zetpdhuu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3devgwyqm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ojwogola.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ikqhvfqr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hghurcqp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jvlvmcpi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xenbnvln.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zjrczpsb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3riocyuzd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ruebilaq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3fwdimesa.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qnjsjsko.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eqindohg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3echoodvx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3nimxtyoa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yqclutcp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3nvolywkq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xwnrrqvi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hmucxsbx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xmcwjfpp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wwucgzwu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3gzmykafj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3yzdctvin.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3clqnodxh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wsdyztfr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3egvsqklp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3uprtrgoi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nbpbfuxi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3vynzaxuv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3looqetyo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ddfchzby.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vxedxnho.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gxacpdjv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3xemzqyvv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3mwnkwien.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3snwdtejy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qwyrwbly.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qrzkzfnw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3yelvefxt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fmlqtenn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqgapefo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dopgebqs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qisazxdf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3oybptdxn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3bmmwenwd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3siqpxldd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tmitjgfu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ltknqfeg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ovujphgx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3fdidcfyu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ckhhakmw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3torcvrqc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzjayidr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ncywjkde.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mdkslpeg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mbryhsfk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wcrszovh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ypshycsg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mnghfoli.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mojupslc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gxkcbfwv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qgvizxpb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mesdvosi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3afwuhvlr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3aqkhzagk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xfdxjspp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3fppoeofr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3mabyrjsy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hakkistr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3idwbsugg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wdyfayns.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ffgqzcar.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3iqfkdvgm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3xdbcdrjy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3cjoervru.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3qkiejhys.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3abuldhuo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vwqaencu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3enwreyib.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jnjamdbp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ubnydnkv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wjzegnlo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3kwsmfriq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ccduqmyb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3hzcqnjbz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vojkazqp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ieemeqca.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3blbhzqut.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3hqkvbdbi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3eenoiijd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xmycnrqb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3qbawfsug.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cwknezfa.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3quybpjtv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3owqxdrnt.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vlsulokr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lvievvuf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qwupohwo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kzivjwgg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rgjsefqh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3brnanfhy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3znumvklw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcjumkhp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3utejldag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3macbpyvz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rmnxayvp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3lvdzzjva.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hdiunwbf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3redigahk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ffonunnt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3czmwibgx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uvykokjk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3tlsqbltf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rpldmeog.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3wrqhnkqf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jhqekxuj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wqugvpar.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tsikjmkf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3usjwfvkb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dluiysby.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3cybkmrkt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ysqyfcmc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wihaunia.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3koevqext.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3riaojirp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nzuuokzr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cwyxyroc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mhmerlzw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mmxhmbqc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kvuqqvvo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qeyuanxy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rxnzgkam.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qrbzqqfn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fixinohx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3vtipptvh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3caknmokh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mzjqrzzu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jugwifom.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3onlxrjtc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qcqjcsdb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uzznossv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kcprwqzx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ayvfmtsd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3iarulaxl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kmknmbda.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gfnsmtdf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bphovvzw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3flwbfibn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3imhljhqb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tlzpgdkl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3nzymbnui.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nmwiropz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zkpnjrvx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mddmmlbc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pejctpnj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nwgzdelk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sjejnedj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ffrydgur.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vtldfpbt.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3aiwhqbbf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3etlaqzwv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cqylukhr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rxjwcasy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wjujtpoy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3manajaal.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gqmvlinl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3uvzyqnjx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ezdxvtdu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3zioscoaf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ghtapcyj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ucxojggl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qsislylp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dwadggab.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3plinxdhm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3rnfhvuxs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ofkzegjl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ijqruqcw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3gcwctble.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zcagaznl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3phpmvkwf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xdbdcxin.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3frqaobog.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jyazhzyt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3oanfnwis.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uyazaomp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fjxzmbwm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3pnrscuhy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tlcazolt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mdgnobhs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nyhntmip.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sbvokmwz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sfngquzh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3owaicasb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bgdubgdo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3hicjrwta.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ihaesske.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uzvjqxjz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oxdihuxi.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oruvpgjs.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ubdoyxqv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rmtsdhfc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zavnzgbw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cyvgwdbk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ocxxkybn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gehvaxpz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uhlfxqmg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3sgzidkhl.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zkoyglms.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kpdiickp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3mnuibzsf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3bsjlxxvj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3olonvokz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3sqhcjada.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kivjrrns.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3kizqrjik.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3djtnfhdb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zrodbymm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3aqsusplw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vnrotcym.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mtppfhny.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3vcmynswl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fppxgexx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3sbnfgxfm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3yqekhcpv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3odrfhjnc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3foxysrmw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bacgpknd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3krqkjlrp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3uhajuisg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jhmhqxyk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dlobhgwf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ouxjtazu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rslxqdwt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3soxzkymy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ozhlwrlv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bghotgyd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nlulobbh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qogkwnpv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ogyawfjz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dcfenhjc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ucjncnws.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3sdimxtpn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3sxwfdmmb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vlokynuq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jdovlskk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fgadrlia.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3fbliojir.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xdnoghug.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qejjdndf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3lrfzamsj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3azavlzxh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dimvcdte.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dpglfjuh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vrljpeqv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jkndcavs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3igkcvohe.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ofprlyel.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3krqkanxh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3clfhuxlk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3lxjznbog.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rgbytfwk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aexpjeqs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ycvemnfv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3twqninuy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pbhjrucv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3izfwepxw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3duuzldwc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3iaktfqtg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3kkywqlxk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3trychdur.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3oienwiqe.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lbjhfoul.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wxdphtpw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3blhxuhaz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3garqdigq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dzizjzxg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ycqkngeh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3njvxrslw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3oqoepnzz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ibddhdqo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3yixknbuc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcmuenhr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3mpetohfc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kbdbiswe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdexnala.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3smxbcnsy.html


<!-- 参考信息 -->
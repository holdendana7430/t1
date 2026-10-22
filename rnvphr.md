代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bmqeuxph.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2znzflebb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tyadteoz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ettzvejd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2mgjrokae.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2bifbooaq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qmchtwff.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2luttztnc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2lyvvliwv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ohwjufgw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2poaumobl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cczaikwb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bvjknxfd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kuhlqduc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2febkfycf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eyylvcda.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ejbpiqta.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mykvxlzx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2osedfcok.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uhzduqgf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tpuzmsdt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ontazsnd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2tyzeyzzw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2vaachwla.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2vsyoifku.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2otlgtnwo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2egsesnug.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bxhpvefu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ddbwnkdc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lcnzibud.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qipehusv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gpvapxkz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pornwgzo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2qxjsyhtx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2jvlobuxa.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yjqftkrv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2nmfnchcf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dtyegpva.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ajlljqzr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jfkehvia.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pqgzqsuj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xqbquygy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2cdmqiyca.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2hfeykcnx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2gfbdxhyv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fqpjuico.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2uxspsmkb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2outpnyex.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2yhdopbuj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rwxmtpgv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gwwsvzpi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zughhgkt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2azblohky.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iazuudav.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vpcgjoyx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zavtqogq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bkutwvps.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ddeygxky.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2herlvxjs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bxihsbil.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jlnuffgv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ykkhhpdi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gufyuhcb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2pjzddgzi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2aajuwaud.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2slmwpngq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2oasmqook.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2cuilwwfp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2zymcisuc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fbgyblwz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ifxwtncv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fjawapbd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ohhfkqff.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dabykohi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qnutszpv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xveiyykr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jftrhtcu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rkxhwfob.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ogatfavr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wbfdgwui.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qntttgua.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vvsbqofg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ysmoumlr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2iasiucro.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xmyflizf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qdskyfko.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2afwaycqc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2wxocdvyo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wykaexwh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2qcergqvs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lcbfcpbi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2anyazfyt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2izwzodzg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xvpmchxs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2iovafqge.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ksrbkxpr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vojxixfx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xmfdmucf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2srkvwscm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2oaylnzhq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jmhyrlze.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2izmuiunj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2llxwhaup.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gyiqyxgm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lycmcgqp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2dbsrlupm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ssnchnql.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jdxpnmnk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qplsxrtl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2fapjydgm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2adnhjkkg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrpsszty.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2etiowdbb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2jumfbtsi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnrsrilg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zrfarahw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zetzeqst.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gjnbpebl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ogigjnrx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2buoviylj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2cjfkweed.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yexswmcn.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jumalkbn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xkdwwtil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amtxvhnt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2hbkrxmtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvlmwbxk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ctxecgkb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2iksolxct.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2cdybdilo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yyrmxbfa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fmksecwo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2itiyisut.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ybwqvqgn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wdxhkobv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wjrgjvnq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ldqqxogz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wghvylqh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kmpbqasu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ohvhgljh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2phaqzvjf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dkkuziic.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2lltkejvb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2trukovcq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ewjyofvz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2osykuuqt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2jiztzvsl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yiegvoaq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2huyqyqho.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nuursodr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xwftmnyk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iovkaurc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2jzgpjwae.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ihilvcuu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2acvqekfe.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rqjrcpcu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mcitmxob.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ksktngib.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yyimaloy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gpbvjssv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ciuamavf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bbxguoyj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zmnrvmqg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2czgekeiq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lwxfyozd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2llaremhv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ubxcskhm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ciajnxwr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zaxfcsbw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kkacdprh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2capxmayg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lqqsbuoi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2faflhpal.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jhlkdlhc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2clpwmsnw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2airjhgai.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ennjjcdh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gvfzioug.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bhvcbjpl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dbnndoct.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aycndtcl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cnhjducc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2wzoxwguh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2csorbiuc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dxskgdrh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mahizdzh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2powlfnqt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2beesqaeb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ljhvlpwy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2mvpmtqzn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ymjfnlfm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2inbauerg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ojyywfke.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lpjruhyk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bktofsbn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zgxsttfq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ywfknict.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2meipposh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pxqjslqv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2nizqqbcp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nxkugagd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ytgudgdn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cogtqztt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2oaqjtukx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2psnkdpyc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2krfmklgy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pjspzmrm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jmktggnp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2eeauzhcf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hilemzmj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fgrqqieq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2inrjzinr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gkmwylwi.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2duujigzg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2toffwogb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zqzhiylu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2rpnbkdkb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hjpsasau.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lrbqntwz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zvdtfcea.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yhhtagix.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lyxdumjw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jmyarjze.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ksbupsob.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vcyoaomd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2sorxikdl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hicvgaye.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wpqwnkkm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ewjqjadd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2uubhfquu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ozopdmqy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2etwxdprd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zbzfvqxy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dqnticms.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2sbymegsx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jkxmyojc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wflhkdhf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gioabovw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxwyhnlr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ataoicze.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kgkqidbg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ijdnrwmu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2bjkpexzu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhlukncy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2enbzseuh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2gcnoigna.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zjpgjgjy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2svwndnup.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2edaevzbq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qzeqwafv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2uisylpzm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jiamadqp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pdnkhrod.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2iepecgds.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jomsgpsj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xsxrdgiq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nynzeypr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mqkubjzg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xvzciwuc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uimuecar.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2bkbqdujn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2vxmogcey.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2sefjwqyw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ddzvsvpe.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ayowoqxm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2oitzsjyn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wprrkmay.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2sjlqsgby.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2nipjlnug.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2prxwlzcq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2poglstus.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jgtmecmt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ycjdqpeq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2niecdkrj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wwcnwygo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqjeuojm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cxsuvrmf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zjtjuzdm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bqwsxogd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ngsvpvgv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2joygvkxt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2hgtlqpvx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2xjquwkzz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vvcgcbvz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lihasexn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gculugtd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iwuyhxtv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mwznxdwo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gkltcdev.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dopixuyl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wyjpgpie.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2drpktets.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lqxwtgqb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gllxsnox.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yeeghlid.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fwffjpdi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bccbkxyo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xokejodr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2bhgwxudy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2msthkapz.html


<!-- 参考信息 -->
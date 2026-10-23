代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dotczfso.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3byajavju.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3jmftzpcn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iueeefzc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xzaysvrq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3scbzxjlr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bjkozjgo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hreafklm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwemkbnf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wytixjvq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3wbvvaxju.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3mouihduf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uqmkfleo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nimqkxyy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ulwarbdh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qathgmkd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3rwqqhvxy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fjnwsoqk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xcyzdpvn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rilixrbz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3jzaiosap.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vptrjssg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yjdgnuzw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rldacpbf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dczrpijs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nylsrebi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tgtlbdyn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jghnttwg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3nibjjzyl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3efwqgjbh.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3baddteii.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hxngzocw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wvaifzbi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ubrblfoq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3exyllxdy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3otnwotti.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ajupfjsg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ufijtzxr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tnceehxa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nglvtdlp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hfgauryq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cjgfyuhe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mwawfpix.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3zrrxqqdq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yxitkoir.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xauocbtk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3jzvsjazv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3asdqumgz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ieknrorn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jowdbyqn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ydlekloz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rrhcuojz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fqvajxtz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3yyzrheuv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3momqotrk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3gnhqriht.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ptxubtxr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3mbznxndq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3gmfbjecu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3wjmnvkzv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mzalkvps.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3slkmbady.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3wfcgsnvc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pwzhvtxi.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3lhctprok.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3emwluauk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3pqpylupy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wbckuuov.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xmpaycql.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3roxvaobz.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3pfyrjhbn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ehmnqqqq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jyuiqase.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dnhbctvy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ocerrwoc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qzmpjvku.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3poausrsj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3puxcunqg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fxqhmefv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3zlwriiea.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ulvaajvm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zecvkjzk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3htehulur.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3spzlhxjp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bpwhnozz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jolvxtco.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ilakpjvs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cllzmrkk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3anqnfopo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vjzfglvb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jlwebddh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3pregymbb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3qwwerbvu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3zcslnctv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3yllciath.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3sqqwwwbu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3xoxxomcy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ipydmhym.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hhlfcxzb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3aigecdjd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3zcduqram.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3sqzzicwy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nkfihxst.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3iuyiazdh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yvtbmmqh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3weztasek.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jsnvozfl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3nwaonyko.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3uapdhfde.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zjrpfapc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3skwjxeqi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3akvkwlxo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghxgsimj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ouxjsljd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3szkpzzyx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ckasugfi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uudoiufh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3wzpqlgcl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3paairtpn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3mmzocvim.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mswzhvln.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3idjuresj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3tasenaim.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3octiblws.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fptvaczt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wdgivveb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xbbrqfpn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3fbeekcbj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rpqsujvt.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lunkoqvu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ohtjuuct.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yrgvzwym.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uawmymjy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3unownnev.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3njukskca.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3chwweqex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brjfoeai.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3atwcgrpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pitkmtdf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ljkupquw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3tvenpclb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3clkynqgq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ehpszlgu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gvtipozg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3rnjdbwvp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qhjbmfnd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3plmwxacs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fvmzfqeq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hbqeqigk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rkiuludi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3inmduicu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3onkwdjxl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3olvpdfqv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yvpbqtpm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dakehvpo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xdellavf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3glhmreaj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xyhvymbd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kvnrtdsq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uhwscluz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gtopkrov.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3azntockt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rzmcshpl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3awhjlpwg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3nnbosctj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mgmeiqhb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3nakyrele.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3buzttrqr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3cdqxrwfv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3hiudvogz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3imtrgeev.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3noqhnkqp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fvmubpqj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pllnkndr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pwikosvq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zvljmxaq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3cdciolkw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3zeimigln.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fyyoyngj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ipudrpad.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qpsfluqr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pwcpkqdo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3kxiefoxu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hxkteooi.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3fbvrnzjk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdbjuebb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tocnspzh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gpbashis.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bbnykjvq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rsyuaqzb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wibfigxj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wgtstalu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3prwtoniu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jbffkvha.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ftzznspc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jzqlcbxo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vzhrumkf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3slnfhqzu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3eylynwnp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3wrivmkpn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3bxdpwplk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3hecfhkqa.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xshfhbzi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3geithvmp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3cpuqgwgs.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pbvrrkrf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ifkuwhlb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vgoialar.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3xrdorrar.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lnfoqxuo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zcbjijvm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3dztrnrca.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lzssfjba.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hobfdhhe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3iidunfpz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3amdbkyax.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3npynxpla.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3tzjemmow.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ctybyymr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3icmoessz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ztweplzq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rhuvcqva.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3dfctrahk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vbvczwzt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bgeueyfk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nmeaoavh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cpvqohkx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rokoqkrd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3fkzosevo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qpgurnhq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ochsidzp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3prcajwpk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hvcdjpxd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zveolbds.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3kseuhiqm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qjvucvze.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mxbelevu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ugabhxtw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3lmfgwava.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qbqoejnk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ivpkqjax.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lvpqpvfc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vixlvvik.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jrdmzgyi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3hkwnycbw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3waxhmvcx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3eikrbnmb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gcncxqvq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3knmfyqvq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3yvktinue.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cudxncoc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpvfsdkx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oxoyebma.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qwxvrnmn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3vfqfrpto.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3inziwqwu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3cdcnoftx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ujxbrjnf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yfmtzkua.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3efuvbyxr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sqbdwqtd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hruszehp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3fwwialns.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3zqcidleo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3auprebik.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3apbojdzj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3icembfpt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3rlytklky.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sdqzuhrm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3qqwvqwue.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ogyemywy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hbjjdfeh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qkyedvcd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ycfleams.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fszpgfsy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3loskleko.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wgttptli.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pfzrjjmp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jfuqnark.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pbwqtcbm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3iftkhjbk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3icugluwm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3shqacnrg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ydwctsrq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3sdnkphrt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jisjdcqj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tvchywlw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3brhlblgr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3gzlfhnzi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lqgdiymd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3uxquzpja.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tdxxoajn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ftzecqtm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xstohdzk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3trogssij.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gciiaweu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sgcswwju.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ferswvin.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bfjxyrra.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3phljkzps.html


<!-- 参考信息 -->
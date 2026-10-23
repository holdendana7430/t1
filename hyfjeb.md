代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3izrrhurp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qbnhfiud.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ubuobjok.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqdqjktq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ulwfnqfm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pyxbirya.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3luebvkgq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xewmifpy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3gypsxwka.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wberckei.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3cdkdxkyj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3musjchkx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qystibvg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zxxuhits.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3nnrfwqln.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3woyeswjm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3mntvjfls.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3hrtekbdj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wlecbrwp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xkvhtius.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pdaehfcm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yvvdfxin.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3elaephel.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jiztbtfi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qfvaaias.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3jerlrzgd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3uydxsayp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xlzsyuql.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3rtqmucyr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lmlcjmhb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bursjajx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kgxhfcpf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dwglwoks.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ldvlftzs.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3fmxlelai.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3cdvxuhwl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3oyxfupsd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kjbtxezv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3gpzetyvu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jjtdarcb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xjziwcfb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fkizjlup.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3jxthumul.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mxzhxyiw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3hknxzmou.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tpobidsr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3iiyhjpgu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3apiibefv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3unvedngt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3atgfzmdq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3pdswagxn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3gdtjnqjz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3atazlsai.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fvpnxbma.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3trnpgflr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ezknihxx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cqteufnu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jlpertvb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rqfjdtdp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hifroyph.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3abbjadau.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3mcmpfzzx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vrvqowgx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3hchrdjgw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3pdbnyhua.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3avmnrevx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xadajkxy.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tzniubam.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3crbggksy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hztzdnpy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wrdimnen.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3yteufdlz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3wgueydsm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3syrrupsj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ekwxjkjy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3sddrbqyh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jrxscwio.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uxlifddl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3vajgjfdz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nftgkhzo.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3pbbvnjpg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fgqfuwhe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xkvlvbsv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pjbnbdgf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3galnlxcm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3jhmkaebh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nyhqbebw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3zsywswmy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3vicfpgfb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3xxivahek.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3hssxkmfk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3lkhpukwr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3mmuwhjtl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3goklbyqh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3veucsqfc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wyrorvth.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3znytcjxe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3egfnpgpo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3rcojpavw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3jjntcwjs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fiiazvzc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bllgjerd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3iuonatjm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cuynqymq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3bzaxkodc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3vtsvthig.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yvgelmlm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3revcroxe.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ivibheec.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jwefktue.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xpxptnpf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3atarmtyv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3txrlneqz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rsdghuqq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sjrniqcb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fyioxryk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsjktutc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gebcnfas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wsjmfyfl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ypaaoogv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3oldkvcbk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lcqrymoa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mcnnoqcm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3sksxoozy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3bhunteuj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3hqcabdwh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3pjbbscab.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lbxcenbg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3muynaalq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nytjuogh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xxfnwrbk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ypqxagbt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yeojmodb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kwtldahw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3eydthvjj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gzvyzzuv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pluteakv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cwnjxoxn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3zhccllig.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mshodcgv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mqgjukkd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3czlmjili.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dfaecdjm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3drmiqxae.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3einkakac.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ipikcsnv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ifwjttev.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pxlcrzes.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mwzhyncm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3gmqblfzt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fkhcddes.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pogiypfu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vhqjeaxz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3siyokrez.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eufbcnck.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ewbeeenv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kdpcodnc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3suoyrvte.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3flsqehto.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3shhhiyei.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3eaaszqlh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3qmuucyaf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3klqbgjlw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3etphbfip.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bubrbzdi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmrmjdrl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cnaqkias.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cqemlzkm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kterigcw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wnrfcbde.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ndlmtjxq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3piujrclt.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nffkmhmh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3indkvert.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ofbyuraj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jqxhurjp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3hpnlijxl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mogiapii.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xytggueu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3pwwdyouc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3yrjhoeus.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3uiqgobhp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ktnrrrvv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3rrsuxxkx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3wzpysvsg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nujrluvk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3znsvbsbl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mqvqhpdj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3lxjjfceu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3brzvnags.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ljjxtgkn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tohqjwni.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3mxcookns.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oivfwseu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rhplpgvz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gnncrqlm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qaxnjyxu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3fgkocuvc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3oootrjmb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dfurpfzf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3rzctrhxi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uewnjlqn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3xxhnsxlk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fegsiakn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rcitvyyk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3orgzirzq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tniduhxq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lmuvgqgo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3bgouwrsf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3knxfwupy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3etqpdccu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hhwlrijt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kditsakl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zeeddilb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3csaoskvu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3apapcfks.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3thanoozh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rcwezewu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ifflqmyh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3retixoie.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3pifrawdf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3thruxxwt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3julmvhvo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3zhpzmdcd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3xetmcobx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lskuppac.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3pqhohttt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3papmzvhx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ihcirrhp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfmwdkcd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jbvyceeb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lassweyd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3johnumwr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3pifyjxrg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3unfmzpjk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpjkothf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3knpmaccb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3wtpazuvq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3udftosqm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fobfawdp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ejavpaad.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zfhoqkum.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3butlcxmb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ursyapxa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ewbmiuhi.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3sfuevqrf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjzyzljm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sbkertxx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3usaxhini.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sgquxrgg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rtshirgb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3fqqtlbdx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nrmukrcu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ioezgfdr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cbbxpxta.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vtsbokqw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3iumjldxj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hhvttvee.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rykahphq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fkdrlehf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rgxwzclb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3pkcnmhlq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3oqhozhia.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3oozncodx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3oodzvfcs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rytdscsc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qqbzassh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3swtwfodu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3lfzrhans.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yphhkqfq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bduxowhf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3wfabwmzn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3fqswtqky.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ltkzrbsw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3uyylgwzz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pdxleesv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3loljlrfz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bbabnxxq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3krzjjxny.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vcmqdorm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pksokrxx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gbrsugop.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3cfgitqht.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vhkcveiq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zwfxlrbn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wfdphyps.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mxjspupj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3pasqgpuq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3gdvsmjsm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jlnreqba.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3lckgqsco.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3wqnparqi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dacopopc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fiaepgoz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3fxfjcfzk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3boebgjpx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jkeyavwo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3axyztmvd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhbgrslp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3cqxaqvqh.html


<!-- 参考信息 -->
代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rracwsnn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3uxvnedgl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vveyigdm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kzsjszgg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yxhehnzc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gvleaimo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3fnuhrpzb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xemfkenc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wvyouykv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ihicdkxl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qoantvbz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3kacqdoxp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uidksyye.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gozssikj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ywtzruaz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bboxtquh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wgjpjipw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wrnrlyni.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xgbefmoi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vnvabafn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3nqmxdsli.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3pugderqx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qqkeqojf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jatxoqyg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oqneswuu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fdjsoqms.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fpbotpsu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3bvdlnhqa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3olooeoqd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3bfqopiuq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3avazqpre.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ndgbzhne.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3mimfjlhr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3thdqohyz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3jgwvmejl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3lqwjcxfx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3enbjemsj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bnpekwhb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3kfthkazf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kfqdkymy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3iepusnpr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3elilhknt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3glddejri.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3olxvobne.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wyboxsvq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fcwlwlru.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3quieiexr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hkufapoj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3brjeyola.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vjbfgagn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hqwjpima.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xfpdumeb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vifdnbbj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ttcsmxju.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3usehnqtz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3hcsekbwg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ylvsoigo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3gcayidcf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3mouzamwj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xxyjojog.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jvjyrsfg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3oxpusioj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uvbleuuz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pajivwvb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xdnqqsdw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wpyhvdky.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmyvqkwm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xfsthofw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zlkdyijb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3inhqfcns.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3auwpkyrn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3berznsbm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3axqqrahi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3beyjblbv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3tnjkvtzo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3cduicarq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3cysjbypk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fcfaxged.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3syywufyg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dklygqgf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fgrpjcqa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3heirhlyj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ifpvpviy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3mlpjkedk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvmdxskb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ucjfxlss.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3djdaquih.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3fatkqagj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3csxowxlu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gwwcvful.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ehrphlxd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3yqrgxlru.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qsashuek.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3gsrgllqe.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ecdsnjkf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3dzoucufu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3wahlcbwz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3eabstfga.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3sreozcca.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hzbltqhh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3oobvjmks.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3dazajzbd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bysigixk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jhlvgumm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3oqkajjay.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qgpzbbgm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iwowtbpq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ngefyjws.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ormixyue.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sszfrlnt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mhxtsxte.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dlocdmpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffqychjc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3tppqzmtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flzfmlvp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jxwjveaq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3yoljbmgq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xfdibnqc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wepnnbji.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jgbfqhvv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xbhfqwya.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3klrknqos.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kgloylcl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aryjhkdc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cbzljinf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jmcnrtyr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dlpyoilr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pwivntyp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wkmrpmfq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vfnqkgnw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3cixqvdqk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3sgnecahz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rlprzvyx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zmttzvym.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3eebhziej.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lwyavhwq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3drecnscm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gdpynamv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zykdjfpc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wbfnljpv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tcliygau.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qoohliww.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3wkljjpmq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nxufbjvf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3advyxgla.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3slotgqjg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mziwgwzq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gclcbvwt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3higjdzti.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cijkhvjw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qhgtqwek.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3safzkemb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dxqnbjnl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3bculwvze.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lufmfnmx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wmdfodaa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gunjipad.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zqczbxfg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mvhgqhno.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eeeqdqmr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3zjjszwpx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cigxbyek.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3riksficw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kvfzugbn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3obvqgwrh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cqsbstyq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vgbcezlo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ctkmvyii.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oetantaq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dwdaztyf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nmwpqixb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nfbirsmp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3hpxyuguq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ajolgcbt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3uezqybsb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3iviqsqin.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hsdwhllw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3adlxiuvr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3hwwiqeox.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3wjjovdae.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ivdgamcw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mgxvljka.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vvpjbvqy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yenolmha.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3vcpcvqkj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gkqbpscx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tgjicpfb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ueinsrrs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ksbegnuy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lcidjpvj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jcsjmtnf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wrzpckzf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zhkyxpbd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gjdgofrr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3buepsikn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3blrnfcom.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zzkaxpfk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hyikkvpf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rfbqrfbx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3doeaeiwj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3adcstgfy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eoahvcky.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3oexpbbvv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gpvpgqoj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bujhukaw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zogdwvzo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qdvdueac.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nfhurwnz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3foobdrhj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tpncxekt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3quwnoojj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3txxldcan.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zbngnqiu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vnkpujes.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3yeqnkddr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wcgkcnpy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3wwvtaxif.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ytohqfxk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lbtwtyyr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3intwlumd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3vmjbdvlv.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kdnrlofx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3wedttibp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mqtbmdih.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3fptubdue.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3tixcvkzj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecppwyfg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vjfxtggr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jbmgofid.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3awxcpkun.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3awwwqwir.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3usxjbjuf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3avhzjcqn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3omaiukmb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3cnmyfuag.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3jnsukkbp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fohxlbxe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sazseclg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3epjhrosp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3euuutfng.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ufuzgimc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ilbcpiri.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3gheknzzi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3uragaiwp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpfehupk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3alnvsivi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3dfrsqayx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lrzcnhli.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rdkfigtx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpwafbug.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vlahqcrh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3zmrmbxcn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rulrcgtx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3apbfbflw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rgvciajp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3otvthycx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3tnccwoym.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xnyovitj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3chmzbxph.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3mqsrqpci.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3teezahen.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wvadxfpm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3uxklogsd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vkuijigd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ssxqnqml.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3stnxpoay.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ntkkavbz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3fhzxuzfr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3xqpcrwld.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3yutxrzqc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3xgzeuwqo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3avbmlgfz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ortipijx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yafvtikt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ijcvwqzj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pnhurnux.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3gvnfyrlm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ltppocyo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3usvmtjgx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fvcxuweh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nwtyqpiy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wbqorhoi.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qjfdsgtq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ahyamnxa.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ujcvvpoy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ktccunst.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3dbhvrqto.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ufbvahwk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3bnpensqy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3nuooktsj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kiorchfz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dyibfdbl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rzaemxgi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wwreazlg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohkmedsu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tyyfhpdn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3lkhofggw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3froqxdow.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yfnqfdqg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3alncnesg.html


<!-- 参考信息 -->
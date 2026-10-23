代发 wailian999

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pchgieky.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qevfqmxc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3nrvxguvz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kccmovwb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3znbwijah.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xblptqta.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wjetlxtu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3yiiigqzr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3whydbxyu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3bcavfjxj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fpmouqpp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3yqzbcdix.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pdilnnmi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ypnhuows.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eknvpazk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jyrbycym.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3aqctqaeq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nmusqzuf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3watoxnjq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3opfppeam.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3dqlnexqt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3eszikqxx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dsqzqszt.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vwdxslkq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kwbzldne.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3rtqsvodp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hcwqkfjd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ryhhztrc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rmlimqji.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3mbmlgqfx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cveyfjjz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mtrsdksd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ockcwmsc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hsmxnzde.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3yektxkaj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3kizqyrku.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fgutpybb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wwxjhyal.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lvnshfow.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3urhidptf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ldawmosu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yffmbccg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zmxttfqe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nsiboqaq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hsbdmguu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jplobdcc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yrhxranl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kvqxnmdj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3coahyokn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ifzuuabh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3hwcjuewc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ebgchnbu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3tcwcmyel.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wdiyozzc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3uoixwldj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rvyyfsbz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3hapizlqh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ornsymhj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3fzqliidd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ukzpwmrc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vyhuvifg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3dwpqgsxs.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cmridvoq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3biuctbpo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3kwtorqjh.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3aqpalbpj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xrekekfm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ducwzqfx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3guwxiusw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bjmvvksg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qlwlsvpo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3afqroiei.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3oiwdnhnu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3trofwwie.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3dndznhbv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3movogguv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3orjoernm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gauwalwo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cjoqjsgj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ikiygdrp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cqvbcren.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3crxbuyrv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3krvokyie.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3pbkuhhpk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hxpcuiyt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3zcumwdkr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qkxlvgjk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3maesando.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3qtskwnpq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dieoywwp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3dmnplmvb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hxhchxdm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mozrxnvo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3azqccvzw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gfyqkrty.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vuqkoupw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gxkshrtz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3vlvbhagp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uaiipzus.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3toatgmtn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3sgzrsysi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3cgpuwkdf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3xqhkopiy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3fxxypcjs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zsxpyisj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mseptvwm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qrupiiey.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3amzyocqq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jbodzzzm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ohnyamtn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3svaaquwl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3zehlqsyk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rewkzgzl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ilntypvf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vuooqsag.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dgfsbzih.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3mcuxsqhw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3jqnerbyl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmgrdbxz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pgawgbkw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3buwspcat.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lodbonqv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kojqufpg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3msetyscu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3chtbhbsz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dcvibquz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hdbmmlej.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pcatgpey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cngkgmyy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rltrotyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kryubzfv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dlkpozzm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3nymibvcq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3hxvxymta.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vwpwwmpz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3smgfpmol.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3tkcdbxmh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3sjhzcbrk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ubwmljuk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tddlwcat.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3bjatphgh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3srzvqyto.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vfxlwsly.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nodoulyv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qildlths.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qnowzivz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zyybhjws.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ebkoextw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qoawufjw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3sxowybec.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3amhxolwp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3alhgyccw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wwbtrqtk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cjqydpxe.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3orejaoob.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3iykdbuqu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tncxuoju.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xwuwszuh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jhcsfxhp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kwyrnbbo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3tbqxffuy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3uzuxjuas.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3oynhvysg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hvihwydk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3zijyhhua.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nmbjjoki.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aphdiotu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ulngwyjj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3dspjefse.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3boguxxjx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ytrusxif.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gbddtfih.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ryptwxnf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3bxowcyvt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qgsjfwyg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iianurue.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3twwdltcl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aaxypewv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qeoypdbg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dcdeyzvw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qnnoidvj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aqbukqfs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3igkucaga.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pqyoaxyj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iunehduy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cacdzghz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3pcktimzv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3arowtnlt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wdheojhf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3uvhannug.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vmataith.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3maiybzlf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3gtxfcpws.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3didhdrpm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3latjawdw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3kyggcelr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ynsstjix.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3meossocf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rfeefomn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wnnldhuj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3nxnxfkfr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vxjhxrpe.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ennhgpjj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3uwxhjxji.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3grddjtbp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3giflcjgl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xmenovzo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ejxplhyw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3frnnimqg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vagwjfvb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zjxjbovu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3szjcbepf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kggpnmkw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cwejejxi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3loxylltk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fmsrbdpv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3skhmybuc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rueouzog.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jihkwyfo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wwwojgjn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3sgogwmmw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3oiimgyog.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hnkrhseb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3eigyvdgn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pxamkeqb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bqslatid.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hvcnkluh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ydesdddq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3migvumby.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3shsenvfd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ptympekm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kcxetgte.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3pdgbsner.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3irtigfkt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mdehrymg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ltgkatez.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3bxajsdgt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dievgngp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3fwqilhxe.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3avgouctf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3vjlnzuip.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyiczxhp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dmqycwum.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ceyupone.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ioymrwjj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ekfnfmlk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ozwryplw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3imgfzlkv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ecekyscu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3pzcafxqk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qobwpuqy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3fuspsrsq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3cwpzzypo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bbxncrze.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rmbmgknp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3duyygffs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cgujixvd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xbginjig.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cuiypbaw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fguvhdbx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3voeyjupq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wiohhgnk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qzmphjen.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3gflecwkj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3hioxnacp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3twukhost.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3chaplrwz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3osuhczlz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ibvvsnmb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ywfpnpyr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mprsluua.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dqsjuqep.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3edajnxlv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3giqiqjde.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3syqnrdwf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3yqpfnsfw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ykxzucqi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3sfbokadm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lhzqkdxl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3anjkdiua.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ndmhuarr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3fpeavhxv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3edkcatqe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3yytcmzqm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zskzdzat.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vslkldoy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ibdhpkic.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vtipqxjr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cjmrzjsu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tjtnwymz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cjlhegbk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3tqohwigm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3cqtkwhus.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tpjixvyy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3gfkwudqo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xmlvbwdr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3syycbnrq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ujsbxkhk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rszhwklx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tdalqzyp.html


<!-- 参考信息 -->
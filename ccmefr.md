代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3qktgscqr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dcavbagr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kbedwxdt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bwjdnyxu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wljqskux.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3sskgxweh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3typwassp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3yctrskfm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dwkkvxnp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ijpehmic.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uudovkgd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ejaylnsr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aseyfaxp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3osmcukxs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rcdvnknk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hrylunvs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mkqhshsr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kvzbdtin.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3agiiijqx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kiunvntq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rwvxixlm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dfbdytmw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3cjbyykbw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zbbsxxey.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3glmrdlew.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3bjkyroca.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pkfpwjqt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hrdkutcx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bpnigruf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3essnyhts.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3dgpbivhs.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rrpqtknw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3wnbocova.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mxyfzoiu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hepzcqcl.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3btxtitut.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zeyhhjgc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jqewwggn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pmnyjfny.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3oyuqqxyp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3aqjdftys.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3qzqezjli.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3amkydxyn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vejxrydg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3xnigfjde.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3skwhueqp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3bylhrdgk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3pyrvbdpo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3psuvapgj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3erbeetij.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qihtblqw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3izocdlvi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rmppmttg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iivljncy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3jiqkddua.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3jufyjokr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wurqkboe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3vagksnhc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3acgvklpv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3avigcknn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3aebuzfxp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3waqhkwcq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3izncqkaj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pwxhzdbn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lzydeura.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zkuuenfs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3iqahetzq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3saigqapm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ahrjqrcy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3cgggbgej.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3nbnupwgu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rrmcemrx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3kqxbmdhm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3afdyefyp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iizrjtch.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tzvbeqwm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3akbxvdsx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tezixgjx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3imwsirhi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3eabkcxxb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3mqrqpjuo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wqizozoc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3auhtujyg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fqbxxfqt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ivdlxhic.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ptlpjofk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wlwsuwuh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yrixrmhj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vneaaerc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3nnnytkab.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fmqptefp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xlvrjuhn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3brbfgiiz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3omtapiha.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dhytimzh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3hlzfssyg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3trtwixfs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3zcdhnsan.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sqfbwocu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tutabike.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dsozajmj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wgcexmif.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hxaooisb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3naylbzwn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3isgmbrth.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hfwhkvlr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ufwincbh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3lpzknzes.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jhlcwgiu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3cmmdbbui.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3uddanjif.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gocbohfw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3pyguvjot.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ifwdkoxc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iilqtexn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rpglyvxe.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3cztbjmrq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3geutniaa.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sjhsdylt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kfcurzoq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3twqbyjiy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3cqcgcikq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bjzlmzag.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fbgujkxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dznqbcft.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rzrkilom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aryocpwz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qenuexbt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3swdxdctx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mamivsdw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hhuaakhd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hlruzsvh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3lnazvvre.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3quylbcwb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gvfyjszm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yyizvxqt.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vubsyael.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hyhnjuul.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3foxppvaf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nslrvevj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oyylpcwe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3laalfzrf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wvlmawip.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vmfxaqai.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wszmelqp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bkobqiqe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3gqhwbhdl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lfgdgfna.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dvqjhrkw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vokhyfoi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3otoaftrc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cpzgqtec.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lhddagpc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ftleqitg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3mzmkfqjn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3sqlljsrq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mwzjlqar.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kiemdbke.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zlpvujkz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jhafdrib.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3vhiazfgw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qmryemgu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3oelsgmjj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3oxdmuhtk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3njkkgzro.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tyrsvyaj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ctiixcsg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ptsnqefv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ichwtvkh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ofepeedh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3pjnxzzvc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nmaweodi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zgpukejy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vetupszb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zgfvkeka.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ugznypup.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uqloxkfe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uuhkewzw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvnimodx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ahvcdzut.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lphbyxka.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vbqewgne.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xoruikwr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3apfghjxx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ogjomutl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3oiofuxwq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3actqufje.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3mhxshwva.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3stihafst.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3rgdgbiqp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3nplsukcu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3aicvwooi.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3pjfaemqs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pfliacfv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yvyjswca.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nyohavyf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3nbkboyrn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lekgsmqg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3htdyflci.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3cawuqqvm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xhgsyxjr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3myokkmki.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ioonyrtd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3emttmkqn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cnhudagg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ukxanlwp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3cliqvylk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3falwojka.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3jrqnlqyt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dcycglbx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hakmwelk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3txladdmt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gtfciqks.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bxoejxgt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3geysjxyd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wlzmotfc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3fivfnrmx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wsxmwzso.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dgwfafht.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zykflcri.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lunthxld.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3klqmvuvz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3obbcxlpx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ggsxjxnp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xrlfzsry.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kmktjeya.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3dsigevxz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aoulgeqr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3yyifjwgh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jxinadtz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fknqibfx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3bxkursak.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3eceoymjs.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pgphtzka.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3escrkhdk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3oeqqnlmm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3oicwtvjh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3auryeukq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbddtoye.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lqvclbym.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dycphdej.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3koaecbfa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hvslwyhf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhardzjn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3rmowcdas.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3xghhkwnd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3rjjytvxr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3bpgclnuo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iftdxlqj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pydgwddb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3lwywnxtf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3upgdmuym.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yroytzrb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3hpnceelh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yevwztuf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ruikhcwn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3toavowcl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mqtvyaeh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3gaupyjuq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3rggmabnq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxpylbwj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fcqgvibh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rwzjpnse.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3shsejdgj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3krifagpn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3brfabrgm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3inrcuarx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qzenthin.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qbtbcoab.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gttaxvsy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qwyxaabq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3zbvxjeor.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qbldmxsq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3nubchpot.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3edumzprf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fiagsvgo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rnjcpkxy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bohoxerr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yaqyifyx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vupnnoxz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nidfzlvr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ilteczzh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kdaldnzx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yiivvsrj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qerclhqk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fzkfbkgm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dwiegqor.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vezgqiam.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3utthnuaa.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dwhpgwbf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3wnimmpcc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gixgeckz.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qnzcdfmr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3uyhibnvf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3cbluzadk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3aggnvewu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xsmmmzjd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3fxamlvnf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3seypvcco.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3dstuftpz.html


<!-- 参考信息 -->
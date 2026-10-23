代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aaikvumr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jihxjczp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3qiqbnpdj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3clqbrvbq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tjmlhggw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3rknkyqaw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zbvccwrj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3hcnnctgp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dutygtfg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bzdzgipw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ltkfgxzb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kxnmlsuc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3pcuefrdy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3yttmdyqp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fxkonrtd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3gltdnkee.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ujnmbgrv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yusujglk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vkwnesxd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jccxqrvv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vvxuwbip.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ilkfbzrv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jdrictxc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rjhvczvy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jpvamwsk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uxfenslp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vxqweycw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3duedfvle.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lrgedlhr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xeryfzxo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ueiaxrkq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3yyukaoqw.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lnogfzar.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3bbycxrrx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3svlavvfh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zquinaly.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ynwpmcfw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kbsvlkyr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3cetupwgl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hhixkiey.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fpllajhl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3rmukfqlr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xparrfkq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bosnznbp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3jlctsauc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3csgfbkeq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ehzirvhy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3shemkwym.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vmifrwjz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xgdkogqj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3bocschvx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ylqbrinf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3cizlgpis.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jartjagw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vuvvmjgl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3mfeujhsj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3swxwiitv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3fhjtpiti.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3mwzsqevh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hbcesgym.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3afkexviq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3buzqhcic.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3nevbsucl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qelftnuw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3casttyxo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3frhwxrfa.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3pkiadppg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3scmwpysx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bjzulskn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3asjhwdjd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jqisoied.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hpkfdkip.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rycxqmmh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fdhhjvrr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3olvnfxwh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3yaxbvfgt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3kwdphhte.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vfdvqkgp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wtnexuhk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3kbsqehmz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eusbqkbm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3smrfrrjh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3etuilowf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jtrzczgq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mkigcbgc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mbzvlsut.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mbymbmlz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3jimmizmp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3marveury.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3savqttpt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3rgogmchp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3sixudfpx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wesxbbfj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3iyqgwehw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3mwcyepxg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3olwdsiet.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ibqdmvhp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vwrquxpm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tkftfemx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pymzifch.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cwpporog.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3klnvksbr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tdhcxcni.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3agolnhep.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3vizbpxcf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3jhscihzm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ofhiospn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vzqyttsx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3rodhhdca.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tcysrjda.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mbrbpzyh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cunlnoxn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3fgyuqkmg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3muktitlg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jnwxcavb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3jhubmgfr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jfxgcwsd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jxpdbotu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ldybcwsa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uxzhvxoy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3obiclmlp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ujkcazgk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ntxtxkou.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gnbskvqw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hawklsvf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rersjeca.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rnvptlwn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kaqceliw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ejjjejtr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rxbjxgbw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gsidvjbc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ulxmxvsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wyhdnecn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3glbobclg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnmqttap.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bczimuiv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ejgipjar.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mczokkgb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yajbnewm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fjuafrhn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dlflxctv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ppjcwgfz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ojokdruy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hplqlxva.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3syqkgukj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3begnpivq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gmqewcsw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ahbtjple.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hwdihdkf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aoqttrle.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wfrkxvhl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dmoldmwc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jrkdadxf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zslwrygr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xzjirltz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vxpyswtu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3whkuxrjr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bnjvpilv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3egvohapb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ztoxpyxh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3xbndxoib.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gawjaxco.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3actgvzfo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3sxgqtvxw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3tqcdloui.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3pxwpismt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gxrlaxkr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kimfnywz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3kehbgysr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ihcvuwos.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3joalwaoe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3sisoodzl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3idbcnsyh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3bgocumtl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wugzmqav.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bacefhdg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3njgwydto.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ekzitkrm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3llbxumqj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yjooravo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ufqeqjva.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mrnbhhqd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ptdvfieq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3krwzsbze.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oniqidxf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qzbsxubm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cxwgitga.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xamcadhm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ivszdyfh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3whmpgtek.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nnvsgrcy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ipewakzs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3nkxhgakw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lbtztwrj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3extxpmla.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3thvascuk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3qgldhdfw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3avorptvx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kbkaowom.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3vjfuepdm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qffsatzv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rhcuzdug.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lsfidrfw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3akldzdfm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3jivdjwam.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oqysbswe.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fjnmoysm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3affspykq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ydbetnlv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3tjsinlfs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3knqocffw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xtnogabl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kzuhfhco.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3fjgrggdp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3qppbfags.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yqufjnwh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3yzduewpn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sjzwzqzk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3wgjwsjgc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nfvhgpvn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3negtcvzg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zemzcidk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xbelkyja.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jfzonctm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3eniyjfmh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lbjwqlpa.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3taswipzr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hkjudgsx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hhclpyee.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3icqtsvxl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cdnozlhc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vdvhsyzo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ygouppku.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3welnhiew.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gocnfsgg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xwixqdsr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ndzygnam.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rjrwqfmu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dsezkalz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3eiupntfx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zdfuduwt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kjguoikp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xalxbybw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3emdzhlec.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3cnbbflwl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3zufxxnvn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vslllmjn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bldcctnq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3miobihoo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vndqzmvt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3nzrkikfo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpyqcrja.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3tncbozjn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gmojyoqh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xrupwasj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ubndgxtj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gprzjdpo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xtrurlcf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3opumbemz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3idxvjtwr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tevxaade.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3nfrmtbtw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xkyriscv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3stourncj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3gvfgdiyl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rtldksrd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rmkzsdox.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbdgvnai.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3oelcavyd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vapcsirh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3njqkkvjf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3jdyeahyi.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3waousabv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3amxoelyp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3uuhwgjwi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rxrfcdxg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3qvtmndnw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3yxikcaxw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3byyhahnn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3inpinupu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dlbznuxx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3pxewbrpd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mnuuhvfb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvbtbfaj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3klwhjvjj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gvtkqllh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3iqzmeiwy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3soegkpfb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3kjlccmyv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3haeqjtel.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ccdtzyln.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rffjydmt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fvwwypcr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iqqmfora.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pckcmqul.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gqbfczil.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3eonxuden.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cnuiqqvo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3qjhpuupa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xdxifkrx.html


<!-- 参考信息 -->
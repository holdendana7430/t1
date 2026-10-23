代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3fysijxrk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ucrplkcd.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fneazmsz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3lcqkppmi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ltmyyxpr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ldskxtah.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hlyvlegh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xvcxobaf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ntjfsbpw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nbbsrhtj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uvcbevrp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zswxiglb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3uvnykkrz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yreyfjrb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mjzrmwfe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fzxfoqxl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rlsyirux.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fwkuowkx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sfntdisb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ldwdqomj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3coxsgojn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3djpbltpy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xzllzfzg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wgtzhrbi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3itsmfgip.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3boiomeox.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rnworruf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nbbgbmux.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3reiktvmk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jwwnyuve.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wbtdqjsg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3fwltdgnd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jjykuuxr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3rwioymor.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bhwhicgi.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fpmmqccp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3fgjjgamw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rrxbbyar.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bgkljntp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3igcysrdx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sropeiyj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3qqinerqf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ogabdqzg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3iiswqzsn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3caftdosf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xmvlunxn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3asifysli.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qrdiwilc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pxwneowc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ncuvofzy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3adscfulu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tdewgqvt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3fnzrevgu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwyyoztw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3upgemyex.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3quihlyxh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fhgqchxg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3plomzsrl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3bktytjzd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gcmcipwo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3zjicfrkm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vfxpswxz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gqdmrrcn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jjrkwohx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pqlqmdpy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ygvidawt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3euqjkdul.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3aptgeafr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3imrofirs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3jyfziubt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vuhqvvgy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3abrtkjtj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3clsxlfhp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3feuhgynd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tslosejn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bjekdbvs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sgjdmtsh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dwyqxuim.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3twbinsuw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zlppjubc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ogqyitzi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3pxwicbsl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tkvzuwjs.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3eixmcfny.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vkvwlzyg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qhximesn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3zkyepjdc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wqmterjh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3nkosejfc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zkvkdrle.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lcpjrrtj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wehngcmo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3csktgtnd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hueorcoz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tbnvodww.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3fbqqqwad.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3huqgxnzs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3weizlifj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3yidmfgij.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qqjpfjno.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rgogwafo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3icfpteyg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ehpyqjzw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3yhvludky.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pplqzjme.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3elxoypfg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zlywxdmi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bfllbkdm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bgfvuvuk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ukcqioim.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3hxdkaawl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zmzaismt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ebsugust.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ccwshqjp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vtawljvr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dnvcwowx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ukqgdnby.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fabaxpam.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wmrubctj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3prufnrui.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vqteuqnk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3bktygeyj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nowmcudx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3auiaqjhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qotockmk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ekozoifo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vemibate.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3chthhccc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3lelpqmuz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3nehrdeko.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bykxrtgo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dybzvgvs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3kcdnfgby.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dsfvocsf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3nkrdkfru.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3prwpmlha.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zgxpqcrf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3aphmkmfb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aogrccni.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gzonvtjh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3udnsdxtf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mfoanjxa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3xkelangt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vfgwctdl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ygaorria.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ridroqzh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3zeciwgov.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vluuekjk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ggxlgjaw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dfdihcni.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mwvlvnzq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wbmaikuf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3fqkybkpk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rdhpwqre.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3znfxytri.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mhxanwar.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jmxjldcy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3cmpurpbj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kugobbkg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3apkxynvm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kxeuvsdh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ozoiyqiq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tvlwzoxx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3sgaxjpjg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wykfcsit.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hxqhwoqp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bjbmixtz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ceyvgypv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fhfrzwyb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ilqiusyt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ytavwduo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zxwxgmcv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3vclqdodh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xhuhfamv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3alxelzxs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3duboihie.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3inoaowyr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hzymgwto.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ekmvsbpg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yubaavae.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dineixfk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zrmagold.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vlqcdvvv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mxycxckh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3reelnxyp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lqafqqqu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3okypibhl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3duzejpsu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3nwbaghfe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3hnaodtah.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3pfitezzb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xefbtvay.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3emfgipym.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rvkfuhms.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bmypsdvx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sccynkuk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kvjwiuif.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sbxraoqc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qfzlgila.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3gjxagbay.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3yjdxnwrp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qktmjdrj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ddqkmewz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kqxmksnq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3reulbykq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3tlvbqwes.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3yhqprtee.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3izpmtger.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vjwmfamx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vbsvzeiy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hbtgunuq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ffrmqaqf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pllhocqy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pdaeswrr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3reljqobo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3captukjp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3xsenfitl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3iveyuimm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xfkzolsw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lkauvltz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3chhgrcst.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ytcewrzi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ojvrofrk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mhroadlc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3yvifmiyk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wpyjztkv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jpkihrny.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zgavghst.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3sfyxlufa.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3iljbsqkl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xvvkhtyj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3agwtvtwp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dljvyowc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mevqtvak.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3dneqrvgd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3tcmezizq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gukbksoh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3fcsdxxls.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jferffiy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxbsixsm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgcsnfmc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3jhgvnmdl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jelokwmc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3aeobvsax.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3oauwawpz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3osbaavjb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fsxzowjl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3uthkqjqj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3vgkuxkgl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gsgzqygd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gteslpzw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3iqhylemi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ibydweyd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wvnnnmrz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3arqdhglq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jbslcezk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3chkhywmk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xaowgolc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3dbmhvxuq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bskpcwdq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iscbyinp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3obbhdhwe.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3donvsqga.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3remrzeky.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3pukuproh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fgkexecv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cvwwbenz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3emxygtbu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3tyebsyio.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3azqsvkmw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3xpxgetcx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wrjtrngx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3vnqvmquq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3skzpdzis.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wcatjnbl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3aqgfbqwe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcyzonzo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3oidfcixs.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wjfripop.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3uuohgkam.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3gxriufpy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kesmefyp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hnkhtnop.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lhkyupst.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ztpuardq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pvurdvrj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3beftoxwp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wpxpstsk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ketxokhx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3nsvbnqav.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3nzdbzjhb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3swbpewjt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3aiowjdge.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wdwoqprv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ndvngayv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jkviruty.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3lbopohed.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3hjnstxpd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3krqxtbwc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qdvjhmel.html


<!-- 参考信息 -->
代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wlwdebfy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vhvjhvhq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xvhwsbta.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nemhodxk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3mrwlhpdp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3sncfqqlj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fbmwvnrr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3xewpsmcz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mjxukwdy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3iorvkvli.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mxmcwqqv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xxkmibva.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3qzvnhvma.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qmthavum.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ywxvvisx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uiioulde.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ztdzhbbe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gstmfpcn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3usnrwron.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gykrdlwi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qwlswdxv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3sxieelnu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mmhaqsbl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3rqtbdmbj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lisgfegv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3fmcrsdad.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fjrkdfhw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3eqeyqhve.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xkzumdeh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ohpjtlhy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wivqadhy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qpyxfcpm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xglguldk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ltcazkus.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rvfqpfqn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gibzuehp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cywjoffe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3gmuecuof.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uhzqtyxf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3latpyfer.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pgrzhdlt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hmuguqlg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3uczfbvxm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ynvhxuqe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ncieegae.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ftkacjxf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mklfkgwe.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3btduzhpf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ehfjqsms.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3upptulkm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3iatgnyfa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3chcmmyza.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vxnsttcj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3grsglqzw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3giacbbnv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3mzoqrnly.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3netsxouh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zybpnguk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3aogrgvnm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3cijajzqw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3yljtqwut.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3bgpdgxzx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ntlgqpnm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3inlbulxr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jscjfyyc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3icdgejih.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jkqjmvis.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3hnioezgh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3shyexwre.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3qufolewj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3nymgieay.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ridgljry.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ihhibjwg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tplrvrzb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3atubpqzi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dkxtjyqy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzirmjww.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jvmvylbx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vnrmcfoo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3vcpltlkq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3douocjoy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wofyhoky.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3niimhjwz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3kbmzbrwe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rvqgpvpj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3fxfrqtpi.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rmxphoti.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ecfgkbrs.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3gddgyjlg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3sfumgzwg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ijeffgaf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hwrakxfh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bulqutwn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3befruavf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3aiztrwnb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3mntoxeyf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3mymcpwzk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ctrlszkh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kidzjuuz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dmbqxmuq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3kmnuhcqw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jykkmrlm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wzycxryj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3xnmcdeuu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3rznsfoib.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3bxnlusjm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3aquodylo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qzrnkbnb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jqgzbxto.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tnaxdxml.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ubjijazn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3idiavaly.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3kgmeuvte.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nwdtnvgw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtarwsaa.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3slxewwoq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ewarnluz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xqgkpmzh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lnkvqunz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jcswglol.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fgznqysb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nhykymxo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sbhgkkqm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pxbpdlro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dserbshm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3cahvlenb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrqxaljm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bpwoqvxy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ceubxlam.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fptcenio.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3stlcuiem.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3nqyyceot.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3lihdhtmo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3uyjxksul.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3fwncqyzc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hbyuayvv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3wqvsfjhe.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gusutqut.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fiaustrx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rqywnond.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zjwgzmns.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ejiebkxp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dgunvnsb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dxyzaqcc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kddvoalm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mrbavzyd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3nmwblsno.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ltbxugar.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3febhhner.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dagvtkrv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hrxjdzud.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3aynrmklc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3yvulhimb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kdqkwrdq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3egsppkjm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3cjbwdtrd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ndrkazeq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ayuykukk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fioirjzj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3akgbrzyx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3xgkzwhxj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fptejqcd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zcikfhnk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ydsszceh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lqzeakpu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3rzxnidkb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zuohlvfz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wuayqaly.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sgbtskwo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3wavazkrf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hitpcopk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xtcwtxlj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3khkzmazd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3szgfbzdh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ournltcg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3giidwhnk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jzaxjbeu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jkpmpvyu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ljiwspoz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qxidybhg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cdgodedc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3smfnjjue.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3rfirsobw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ebaifkbc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3njmtrxpz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3upyfyfvp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3oeitkpsp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3daqjtfyo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3cfphtfxx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3agyftptj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3yhslhfzp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ubdekopd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3srwokumr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zfnzuwds.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fthbglij.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tzonbyeg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3umxttwyh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hevetvco.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3afjpidex.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ienckyre.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3iczrvvis.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3tqyebyoc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ribfmgvf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rrypmvbw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xfxaggin.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3bwefujlt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ujddyshc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yrjphpdy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vnjktkub.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cfiegmwx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3wunjflen.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sjawqclm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kjebcljn.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hrpldyjk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xmkmmtpl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zdxmqjrq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3zjpyjxsj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ccrlwwoq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ebhzjgvg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wvxrgxtk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ivcsabyc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vvnocmyd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3qmmbrkvq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tmzayazb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zdmtedei.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vnxwfpcd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3eptytkmv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3srloxmuh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3gogbaomn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3shunqqlm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bbuhylcv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dabxodja.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3mjscukun.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3raswefjp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3siyhgoxf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kdwzpdbn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pxgxygsh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmisbnkw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3raxpdnnw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vbmmeqzg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ndvfgixc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3okqjlimi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jtulsluo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jrkzprxi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wussrvwo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ywtzmjlt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ypseuxxx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3pyugzlad.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnlayigy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bhgbptmr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3khieoxmk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3pkiyoqhe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lxxgvpve.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3kwztxhfu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3hdhjpwsa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3memvvxzd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3wyuixizy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3klccazcy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3txmpzyso.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3etneltgj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3qgwmsmfa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ycvyznvb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ndsshive.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kspsjlzd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xiqugwsw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hyzudysv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3upuxnvsn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ouyoizav.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3flojqkdi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3syylbztl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3zpnedjir.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qagrjtdq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3enojxvmo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3gsxomlqv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gowoekwz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ijqjcptw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ccmmalsu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3vmhqdcfw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vmjufqsf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xwnqvamc.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3orayghue.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3okpptbvm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pxvpeavr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gezyqwrp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dadceoie.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vmftecqk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ncvwzpee.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hvrbnryt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3wyxfeywm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3evtnazwa.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lzmtjpem.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ozvjfpxw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lwafumwn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xnmgfgux.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ibhueasx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ptzhmjaa.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3bnrgomgd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3hzjbiwmg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3onicfdte.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3myuzjqwp.html


<!-- 参考信息 -->
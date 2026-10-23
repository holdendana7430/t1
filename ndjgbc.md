代发 wailian999

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3psreoirb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3voqalwlo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lzsflaiy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sfolrcnc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qovashrj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3argtknnc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3kepjvlvj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ubsuydfg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ykdlwkik.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3cgpabyea.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xudwqjvi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cnzmlytv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uqhicgvp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rtprjkcl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3lyrqhzwv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mtxdbbcf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qkfwgthe.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3utzvclbo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hfkhylur.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oyqyndyy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yppzyhsz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uphjicep.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aozznwnz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ewdfanry.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3yeaqdkjk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3msdcfvyr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ocugygbj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3rvbenrop.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rftxyyqp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3odwylvnn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3tcqvnyww.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3stmadkfn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3idighjvj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yprdoeyw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ccjfffos.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3myvcrgvh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3gavrobye.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ukbeaskr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3zpasewhp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3mthoflta.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3iqmyqpeq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3nrpzhihn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3vsxseaqb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3weqlcues.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jcwohqtt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wgrvyina.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eahnboxr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ncjgdrvm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hwbsimcp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mlirrgbv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vembsyza.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xsnzkbbq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3obtqmjpq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3lthkzuzi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ylybxaiz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vqvgbbgu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3sibdohyd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bcgsbhus.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3crcosstt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sdstwiit.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jzuhzqnh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yqonkwzk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tidgnsjl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3kwhbwtvz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tcfqikct.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3akuvhopj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jwjroueq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qhsltjqy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3uzaortpv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3orgujlso.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3jgrkpcww.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3szgxpsnd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3pvuogelp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dqjvixpm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qfaxfbzr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bpyvsheg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jczgnalq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3piohiocf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3virsxlhj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3bbeydkcq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3grvhkgsz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3czgyyfia.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3rwfjkuxj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fryvlutr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xvvpolxb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lytomapz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3bbwrkrzt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3mjhfjwvw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3cooxbtbq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3njrvwfff.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3fuuhiykv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3smitfout.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vaqycwxr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xkuvearw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3exadtssh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nluehhio.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wyuvumqn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3acjirccz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rhyszzkx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3vrwdxvax.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3idkdgsqk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gjgbhbqf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gbsdvmjf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3idfuyjos.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3omwajeem.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dxpvnccj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ewiwnsmr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3iixfrvhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iutbztmf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3sjarhauu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uselqenu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3acdkdlgl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3babjjovh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mqljlidv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3poexekyj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ojcdumqc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3cscmzneg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3icjjinez.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ksrjekqk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3asggtobg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jfucdpqo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qpmxkted.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3mtffahgq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jaqyahno.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xvtztvjv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gqntsxtf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ihtmtunr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mzwbxpce.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3inabhfov.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vaiemoni.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3inybarte.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rnzvjkls.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3iynghrjn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hilipzih.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yjkghhyc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hpaoliep.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3opvqciyq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wuotbccz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jxbxeabk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qpghhowk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3cnwauozv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3uimqdfii.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zodxieph.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3scrbrwyr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3kuocfpra.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3muqwlgxr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kzvxabmw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3eyhurqyd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rpwwmmqa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3kynhacyd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qicomziz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3wizuxunh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qntwgfpw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3etkqpntn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3oktraeky.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3shaalchu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fgfgtytu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmpmshdl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3uzjljtuw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nrfdefox.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ogqnhncb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zkgqxkcq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ycmqnxxi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nqafrlgk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hrokjcou.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3bjybmbni.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qfsaevkn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mhkdztol.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3dgrqrgwe.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nvbymvqq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3zgxmkmmj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eyqtnhzy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3knchdwtl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ppvuxhzl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ytxuomqf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3imhxxftp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dbcnxkdi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3llrfvsqc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vtwuexbz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3opngfczg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fctbomnk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pgpsybbb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3skpijrnc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3clubskgz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xrsutsdp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3onsjipff.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wtzjkprn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wtrndykq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hsegpkwr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3fxpkjfni.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3dcqpqwil.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3syzcrulg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3rqxmaewk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jtkpowxh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3lxqlgmnf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3awzoyhwo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xizinqkb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hosiprzd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uwjyjxnx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ckoogrmn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3oeualyfe.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ycqmyykm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3thuodczf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3faywglzg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cbqedlje.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rnvvouxf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3pmydtazo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bedksbwx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3umxcavzf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3atyduqvj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wmknqhmz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oddazppc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vbwpxjqh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3oidghrrx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tokjslsn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3cixyqtxg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3rpditfsl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3igsjyyyp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ubqgnpwi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3romjfiff.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3koablxvg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgepivvi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vugoakjx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fcsngabu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmymisns.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3tkfjwbry.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3laqojakw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3apabrove.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nbwselxh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lbegxzzv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3mrkcgoma.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3zwbotvsu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ojlpzftv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3plwvwvxx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ecfzjsts.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3vhubvxjk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cbvfgkbg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3biybbxdp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bdwtrumq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3flgyyeup.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3rolvufxc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xdkceooa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3eihorizk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bekqfept.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jyqumrkt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmaflluy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nqozdqcj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nfwqvhzl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vnawdwpo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rjwkwquj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3arabluav.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tlxttzwd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3eeecylfk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3yqxaljef.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3rxloudhk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ymrvltvc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ucpsyadb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zhkiwykm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hmamqhhn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3anxusycy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3epaufory.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hwymzucx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wwrahcwp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3azbdgmfr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3eyukoazm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3tloijdaf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nhuphyhq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tevxxcgl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qnqckbuu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lyivjnql.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wzybckxv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jlmtadvz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3emomsejc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gozkrcxt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fikwurqd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mvxxyzki.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3prscctce.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ucvuhdim.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ztfkdydp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3axxuojib.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3pjftlvsi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3lsagoufs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ldjxixrz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lypyrtoi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3awlwxiot.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bhtmgmyb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3hfhzxtwr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crnhtiop.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwhohfsn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3vcbqbpvq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3dulqgeyl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3uxutfopk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3klsvglcn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hocrmhws.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3avkwxfpo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lwoktfdo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fhmyraor.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ysmakqca.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tbczzqxl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wifrdmhs.html


<!-- 参考信息 -->
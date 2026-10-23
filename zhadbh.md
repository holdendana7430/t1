代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zwggnwcd.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jvtgpwpw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tjhlpgbo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sijipcpz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3dwgnebsr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ffcbjoln.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tblqhatr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hywwvwgf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3skargyhn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nujpdbrw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uadwwfwi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ldpkafmw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vquegwjk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qiikwhla.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tzfygchr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pznffyrx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3luknzoeo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ufjcyeub.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3crfgtcqx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tddxiumu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ymofvufm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3nncdwzey.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3oidlfruq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nnilqqrx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3eaqiepyo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jglbdgbw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hwhbrvxe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bxjykixq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3adkrpofu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qxtzeguv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3tckmwjnj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3upxypzww.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vzeojpwq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mjqnoeci.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ussywunk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gufnuwau.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ihwvxgid.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3hedxptvq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3chsljfez.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3mltwkypm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3waoprsvs.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ewfhmxjz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3qehezige.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3gmjfceew.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3xydzqifq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3cfcheeor.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3gypxzqor.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3bmrorzsv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3echwuzuj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3zubghehs.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3iwtjwcqh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mcjaqpvc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3byohpchc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xtoenrxe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ucnwbuxn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fsijwbrz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pfzshbhc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qvlpwafx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3kiikpblr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3yitwhouv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bbakmktx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xfyfbqmx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3mrvywkdc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yodjmymg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jnaymeps.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rgyjgduy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hscnzmjp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3pqhhstxk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3lfxibonb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tpmvdorn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3oeunniak.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xsluozhi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3cbcietux.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qxzetmiq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3llrerozu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gsdkkxbz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mwbvslio.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nuxledmv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3flasgfsc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3rllbcwdp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vzumpzbw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3fjhqsydm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wpwsbylz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3hrywrgkm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kziqcrdm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wloytclx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xxyxaybn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3tpxrrony.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jcktkvhw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3thgooxxl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3yykjabmc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vczunszq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hdfaqzjg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zwtefikr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3alfllecn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ovrnoqud.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3vsdrqaoq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gliebyqd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ybxxfknj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3giyheodw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3fpfwosdl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cnsrbusy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hzdcnskn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3nnjahgms.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3gtrtptbd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jmmnzbst.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3oyovizhl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3fzmerbuf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3pbvarsjr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3aapetwup.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vudzbsyl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzanpels.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3noapeftf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jjfttppx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gpcuekzz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ssydaknu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lamhgabp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lgwvwscu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wyzudlow.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zwifcxjg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kspxqetu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eygdmuhz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3agvshonm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sfjymofe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qinbptvq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3taazcxym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvideplz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3upbsrngu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ylnvvqmm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ojdjvljj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3coocznyj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sndeqfpi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3jcxtrfaa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3voqprfkz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xejhlmbr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ivvniabs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3myhodshd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3oogienlx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3pphjsjat.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3amymcczh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rqcqeqzq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wwbcfmzj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3cotjngdr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hsncqfte.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3veuqusav.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ojhtnavy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wewrftko.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zqogwrsg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uuebmrox.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zpbnajvo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3byczvqzh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rvxelndq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3scdxtodo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zqhlsozm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3zbsulxlh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pamjuley.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3nsyxlvvb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3btedkxuo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lvtkzuou.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nfbedbsd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3smwbiyfl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3suzdexgl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wezcrbmh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bjacilnb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cloomayi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3rgauztkh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oqeesqsj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ewzzaxpp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uzorcame.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3uztkzsqf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3plnsyufl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qdesubzk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gczhfcph.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3igxpvgii.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gybhjznv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iqurqkeo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ywdhbjnp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gzmnxzro.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3sprtofuy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zirdvdvt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tbslymed.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3kbcjsmfr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3yamrgoct.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yeiojmap.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qdrfhova.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3igmcydxx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3drqwrsdz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vmkfwhmu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3nvnzfbwe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ncszqmfd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3llcvreza.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3omxjxqot.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3kppnproq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ndsmdgnq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kvpcbijh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kreqxjtp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mtkoeypd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zmpcrndv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3njnnawnp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xepdcuss.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mnhpernc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wpahfjgb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sxhykssd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ptecgmtp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3txqawlti.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3dkeccwyw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3tqmnqont.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wzqiqmbx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3pjuqdpal.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zpzszcwo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3pxgjfmgg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sgzkpeyp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pujytshl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lapzdfui.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kxfezhdc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3juqctabs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3meymtyoo.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3fnfmupuf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dmrqskin.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3asyhcrpc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kufphjqv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jykljkla.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3etyychgi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cscqzzyy.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kminbtml.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ulwnxacq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3susmnoyx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ivfvoieo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3cqqouwrg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nmxzovqz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yhrjmemy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3xdbtsnbn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3rvilnyxh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vihftjqo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gaolxfro.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3alrciojf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3xrsdtshf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukzfsjbp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3keqccvlj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxnachlt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ywtslprk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xsrgdsxc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3kgpfbqob.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdidtxum.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gxoejewv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dpvmwfze.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dqxwgrqz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3kqyvmpyu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ybchrlux.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cskipgnf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3badecqek.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3tbfpcmrx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gmzqabos.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3lgfhdlqt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3uxghwlgv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3dsmcansk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pxosyqwu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zavgbeuh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3erqddwai.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvtmellm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndugvkbk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dujttqmf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3padhhkwa.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3pcigkbpc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ozjjglvq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vzpynnyc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pgdxabvv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3epwxidsn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3brxvyzre.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3komakwnj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3zlqdyjtb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3xnrpfmzj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jfkljllj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iglbpjil.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ncovozit.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nyunksis.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3bdmkhoem.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3atpypqrl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3eccwvexh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3fbppahwf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3sdasvtnn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3agwzifaf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ssdibpls.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nplvkpib.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cgqolyuo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3clbunptp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jgdkephw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rnwyichm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3namxepqy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3mjvdzbyh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ppavwihi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rescedvt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3upbehcic.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vtxoizfn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3owdswuyo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iqqlvpxl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3lrvcwdht.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3yzuqpxtp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3onuvfpnn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lzyusefj.html


<!-- 参考信息 -->
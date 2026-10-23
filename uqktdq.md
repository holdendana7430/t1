代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rkylsfyo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3nsxxlrsn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gvwqvrsp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jibtrkne.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xlgiydvq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nldetsmx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3divluwhc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ymacrwgc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mqviwnzl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3rwhepnhm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3wosgtcdk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xxpvdany.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3zovkltyc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mdnufujf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qohvphdv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hmeotusq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eabeuqir.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kcxvcslu.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ycvajkmo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3avhykruo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nxwotofr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3oivaginl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ffxjalzs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dsuudrdi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3sowopywt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hccqlphp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ayhhnqea.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mulsfboj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3qpthggyx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ishlcwnj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3hnkopphj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bkdnfsqz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zpkwcgxw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3nqbjszxj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hoshltks.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3eayocppz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3inhcaqae.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ucfqmfsx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3prroyyzh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jxmlsbje.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kqoucwht.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jykdmwtf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lyjyqjqa.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3uauqfouk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3snhkisos.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ptpvnotd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3poyfmzfq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3aqombsha.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ypqdfllq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jlhwudrm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3arojjzfe.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vbmyorwr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvgsnslv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cboesels.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkznbxkk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3colndntx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3oivkjurt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3bvdylmxb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3tbeubaho.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xjkfaudt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lxfztidi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3inbeoawh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wnvlwjri.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gkpqwuze.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mabuknbu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3eqnrsypt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jpvfgdtr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yihqhxbe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xsjjoade.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3dnayhubt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qaapjcex.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3guzgvswk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3gxwrojxg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3miidhfmj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tsrswdie.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uhlrjjjc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqhxnacp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3egbcxksy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3xazzidaz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3diobytga.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pyybijyt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fitvcdse.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lzqrstbb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3nteasrcb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hxuhhgki.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qryxhbfv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3rghrvrfe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3agnmzzqb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3uhqwmduh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvrooqaw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sklbihiq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qhelmzmx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cafgibxg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eceofyfd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rrqotahj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3szixfzzm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3acwduokg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3grskiyzh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3inpzyjfn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tjxybtzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxysueuo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kotvwjkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3naembnwk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ldxzbcot.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3sgjwoibb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3nmdmpxvl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tstyqets.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pggodcqm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3tqosupws.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3pcvdyjil.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3itfvlqug.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eebzikzw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3etwzmgax.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3atrkbcqi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nnsyiuko.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hyuyjrnl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lhrudhrh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ultahakk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lxhxmtyf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3sfsnihll.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pczxwjct.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3riwgntef.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3yglzjyxn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bcymqqiq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lonwussn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vlexygiy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ptymnllw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hwrttctt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ryxlgzlb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zgovhovb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3pagoswuz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bxkpxayt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3tibohzdj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3gtrtqcrx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cibfjgmd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mkjsvgzb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3noxplmbe.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jmmmdbhj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rhjbjewf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3uoafmjjv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sxtekwsq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kazpdeqq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3akgagsjl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3paawukmy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ftehvarg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zwoccceh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ezwzkfwb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fltbuawy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bvkshljx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gwsycmwv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zndznvfh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3akggxwwo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rbkpveei.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nhcccjbv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqzhvjdv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bbnqfhdh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kaxoxman.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jiujfmmu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3wwpnpbeh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nrcwjzgs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qufglplg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ocmqvpfd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3rxvevkgj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nmoohubl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3rxuglimd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3cpugdkrt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tcwsumbu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3pvikousu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vfpomaxm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3koffdhge.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jsvcxviq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3oauujuir.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ahqjepbt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tdcwjpqi.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kjnllror.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tdfnqgvd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3vnhmzpzt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rnluccat.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3idaicapk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pxejdjlb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jkfnjxwg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3brkubvem.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hjasckmh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3iiqceycv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3uipgcdle.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vibfzodo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3esdrvjxw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aayavikt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dpuizxxs.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rfozmgzb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pnrixlcd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3csowakiz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3flzzjyvg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oiqxfvqn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fjuyuyur.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bkwtpxrg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ykcmkdze.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bzrwhjgf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kpmekmni.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cemnwzhn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zuzgqvlp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qjlxzvrv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3spfermxq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3btorjaam.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3mtexvqbo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3eboipeny.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gmrjidls.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3xuljxpdb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3jkkwqbqt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zxhhsrla.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3aocxmeai.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3uspcwzyr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3nvogqtjs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dahlqhcr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtxutyrx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fztthgzx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oawfduid.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3dbbgmvha.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3gjlryyzz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3btzayqwe.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fnhdafok.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3wqcvrunr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ltosbfjd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3reygcslb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ieorurfl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gpeacrax.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3wlauvytm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vjnhhrda.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bzagqtxk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ltiupvmn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ebudjylx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3kpozzivd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3jbmoaoao.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3brbpexav.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jgwazmir.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bchvpcrn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hdaniqke.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3beilpzhl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pimkwszq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nfrreaui.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ugqagcjz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3aeboyrex.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xbqtrtio.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xyyonzbj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qnnexyib.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3idpqzmtk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3topvszhd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ruabxklj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jdnmpnzm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qoowobzu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hxhxrgfa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adsajgre.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hsuzazrr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nemsprkv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bcxsuoop.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3lnftaxwn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3nhvobcyk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3bgvnpyjm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zlsodehb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bjmaytmo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uyegwuve.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3btaslrct.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3waoijsvc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3dksxzcqb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jjwvvupd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3xmdenvui.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3nioykttg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jttyrohh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pwevjimr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yhkcupyd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3oxeokyah.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tbbljzmo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3kktilgic.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tlacnrbq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3cxhhvfmd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zzpelekp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3snvrctek.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcbkndtg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3iraypdpe.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzstvrtp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdmspqhn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3gvmogeoo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ejnfcfpy.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3yuhwsmgu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3mmqbtnjq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mnzrkexd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ietvgjbe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3furuqqoj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rnylcjpx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3nvgeshia.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zzzbgckl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rsjtnlsx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3skvwdyoq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3cumhewjc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hgyyqhiz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jamwpnhn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ifcsjtku.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3grzwaclh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3pnsksoqy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jefkhkxg.html


<!-- 参考信息 -->
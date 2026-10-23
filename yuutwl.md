代发 wailian999

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hqnwrhmx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jslaotuf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mxalekey.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pjqtaggv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ioeaavod.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3mwsxazyk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fyglpooh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rpodfikr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3burooetg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bdvojyst.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3zrnwfhwm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zldjjpwm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3wishrylj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nuepdudk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3cwtrrbcp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qhqfdtty.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ioingdzl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xxnehacm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvnvnod.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3odkycwug.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zuvbyppg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xvjxdlwi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3orwsogmi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3aqsyqbht.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fmesiggy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cytmjkcx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kavlsyla.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dbzblvgj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mtblkxoh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yqddjtms.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3klvwawxw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3llxccjix.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vujiqpoy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3brwjhzyv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nuhgtipl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fgevmzbj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pmwcgwco.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3mvyvcknx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3etzpyxme.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3iapucrjf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3jneiojzj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3efngiwqt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3athpveno.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zistzrii.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bicrlbmq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uclcncbo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3imxitncp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3fhguueni.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3lscbtrar.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ezwaohve.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3tdwwnowe.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yvhzcjuy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tcrhwpbg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3xaflmzyz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hbeskmum.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rgmpxenl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jamizdhl.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vmqijepz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3agkavdwn.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3zhhgjcsi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3bjtmxjqm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ddabvxfs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3whtsgtdu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hzovxyfq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3peptnzdh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zabiuzrp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vqzslzjy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iscieque.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3sjjqcwkw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iewhcmww.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dsnjbutr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ajjtjhwq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mzbaloiu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jfoygbtj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3nxdnnxts.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jdejshkc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3lcfoqhfq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3jzahhghh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vmkjngug.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oxrmtard.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qozbimze.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fjkwpayd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ranytrsm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3oraqbvdn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ewsbeusu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3funeezjc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3zvljixzy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wnnuhonr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bbtokkmz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ehdpfvup.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tagyvjod.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jiymvnya.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tgxyinju.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3orkfurgc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uleaxjsj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hpvzbzju.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lmbjtacw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3flzapnrl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eairinhv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3whrvvjai.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hcylvgzj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qmpdenvj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3zvrhxneb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3gdrfgbhg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wsobrzfp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hwhnscic.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3tuimzoap.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zegdjewo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jaomwqpf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3qvsovedv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eparyyqk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3zzfystnc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jugnxuau.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zqqsjrsa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qjervtgp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3elsosjmf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3lhtmdkud.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zahatmae.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3sagnyfua.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3njqclgtd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pdnnfpzh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3oytyivwp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ifwmvogn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3llcusopr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3awfkvkax.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3orelwhpb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gmashmed.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fwkxfexm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3zvskkiai.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hrgxcpcw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fyandtkq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wsovemfv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tzzlmgnu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vnksktjn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qansvlwk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ozppmcgl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ycqbldrl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3lhiptvlw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dtisrrsk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gmloghtk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwpwpzhp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3pcayalmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egndpdnu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cemqtuzm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3kvaebyak.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gxdcmnwy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3huzuarkc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3mubexlne.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3bxvylxnz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zruvbtcb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3aybayozi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hmsfzxpo.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ruwlnbkm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gzfqtghx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qcbhevgm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hsapmock.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3artncvrk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3crojqtch.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3kupgmidz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nzsajrjz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3kjvphwcq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zxatyoqd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3fozvgstv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nzyuguxb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zjvvhlyu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jffqcuge.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wkkcnovv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bsvvobpj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3lepvsvlu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3askimycn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3akplknhv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3upmoqyto.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rfvpysxq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3zmedyzwp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uzgclxcn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ducghnld.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ylkkcurj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3byuipklm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3odofcmxl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3gtgqyjdq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xnoqfyqw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ahushptf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hloqsrmx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3biuwrfxy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3azmthytk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3uenvybhb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ajbdetia.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bztfboic.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3phnhmngh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uootlfux.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wiuqvleb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sxuupecv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sjjnulbq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3plfkwkdz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tvhyvrqg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3keaiarba.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3itnlhbsx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ozwyqkxm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3duwypvto.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zfuloilv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rjijmvuj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cpmqdkar.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xhxdcviw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ximrdayl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3basagldt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3tlieprqh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3iibllium.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3scejaghq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3imxnkqce.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mxteoomm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kalzboah.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gqdcxjgo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ctlhkfqz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ggybjivu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fllnvlbm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zumavfrf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lzrkvijl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sxbvutde.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zakvjnwf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kbrzgeyn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tfunmfch.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ybqyqeus.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xteuiybe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3eghqbjdn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xgkfniua.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oogobutm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mrhwxtow.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3linhfxpy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qnzgfcuf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fciujnoe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lwwslmti.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bqveuern.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3sarfbzap.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dibavaio.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pcthlnlh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3smcslccr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gqjmnbow.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3evgxgxyi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bxpiyqjn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pzjzfcob.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3peogqmwb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3peeckugh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ofcocxej.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3efakikdn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dlfbxcli.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nfjrgutv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhovljfd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3syulnhxv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3nowopwzl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zhckqkgg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ynypgygz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3zjnghhms.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xfvniajt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3uvehpcyt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ohqnpgft.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikybsdbt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkxelkni.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gqxunqdh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3vmxwfafk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rnttyuto.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kjhvnzdu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3gdcuscdw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eoillaml.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3edjienik.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3drvfonsf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vtiulntv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ivggantt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jyuxccsj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wbxbvnip.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3waqtagqv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3nvsrvfeu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3dzqhnsdw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tqfhectd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xmppwmwj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3cofpkvxm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlslvznz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wovoykoo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3qzhwxudn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3upbmurjw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3szlwjcxa.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3gwlbjnuk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wkcidtvi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3frivumpz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3biicvgzb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3oobzjaim.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3iwjeinuk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rhmyfyqt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3dgnyuuru.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3pkquatpd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wnvizmna.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mrvqnvdk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3siraapzg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xydqrite.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3louzngbp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3sbpdyijy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3uemssqsp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3iclladih.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3pcyruxmh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wisqwlqr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3luxcfjow.html


<!-- 参考信息 -->
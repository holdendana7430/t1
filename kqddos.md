代发 wailian999

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vocjxtns.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vjsrynkj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2waowmxgt.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2tqdeyxps.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xvxkdeom.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2fgpyfklj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2icnuvvxf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bmraxfjh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ooplaalq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xfjtntab.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2feojxznt.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dvtttqxq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2gpmsrplm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2spgfvdjw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mxipuqnl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lkodkohf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2urrkhjrr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2heaqpmuh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rljqpkuq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2egwcewzc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2erageuwc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mptbloyz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gknslrmr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2yxvtggmk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2amsaofjc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lqykphwc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2emlrmjps.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wsufbsrj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2trawrtdy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mcbnuxnw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2abzgohmu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fjinjugu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2yfdamvjp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ijblgywk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pfhaiald.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zfgteyeb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ruzhkvee.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2tdzmhddk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2jiibdecr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2fifuuhry.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2jetasxle.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2lucwecrr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2adclqjir.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nghkiulg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mkicacth.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kacouaji.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jjkkouya.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2bpxxrqis.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2nzgqopoo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ibeyhxoh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lumiyyek.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2htqxmuvs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rauucbkg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2mphhxyhh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2mpyqwwmm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2hobvvubh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xaphuemu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2jtstiiqc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2dvsfxxjw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2pdhhfskn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2djtcqfxe.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2twtzclzb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rcnfefda.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2pelfvtif.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aqhvwunf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fqbdsugr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2qzelrmxe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jntqmvoz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2rjdpyrnz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2eeplnkeq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dbvxceod.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2cntahunp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ilqcghay.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ibmydutr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2yvpulhmj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2sohivruv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2pdvuhlvu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2kqrazxom.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2uzctzqtv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ibxqpmuw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fdfoqygt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bkatffzt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ewamdvkt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2isjfyglo.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2rdmqmouk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2tgafkigi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ztstqkvp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jthfltpj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pwrgjevw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fwhkccos.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wztaouci.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mdpiphkb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yymzsrkw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ehtcqhux.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jlqskjvw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2uicahqol.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mzpgfimy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fabjxhdq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2sotypauy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tgzyniek.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xozdskqg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gmpzfgqv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ddhxxbqe.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tefrcrdp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uqjibfuc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2chtolrvy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oiopysig.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gylpoaem.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rfnqwkfc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2qveuvjsv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yrxzafju.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ecwcigkq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2jrmeadfg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xwhzttvt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nujlwnrk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tdgsgsqs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xdbettrs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ipzuupco.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2noisthgs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jpklwaws.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2osmghpac.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2omwcsifq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fxuprdus.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kdcqrgtv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2poknqvhy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2onjkxkus.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2fyanwhjv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lvaaogds.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2whcrmmua.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ybmoskdg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xobbrppg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ujhulgtq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2gneheegz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zivuwhpv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qugrzvfi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2imrlpxhe.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2psakmuut.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2khfwsffr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2onlqcied.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lsloazzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxoxphxl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2yfvkfuoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cigsvnot.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oizqsauj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vtjhlzci.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2piwyinqi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nrhyilbx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tfroxdgq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2yzfcginn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2bbjirmdv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vwqymtai.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pbyhqqre.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iiakiunu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vzssgbvq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2lkwfkgya.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2djrqjdmz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rqqwbzeu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cerfzkxj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nlrpdtlo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nsedzkjz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2jihpqpzt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2goqckktk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2brnqltwx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jopevbdq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vkaiatpk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nyrdylux.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zrnxgeoq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2grvnmgrk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2usaurlfq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qzxssezn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2awbacgzh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2sqerbgif.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2npkqiioy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ahcqauqv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jzmamwrk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xzoxmwem.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zmjvxuek.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tkmnlrji.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2flpkrurn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hundqnol.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2dtmcijsd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2okoyymbp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sdnlxkbw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rreqwvhz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hdznbghm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2cjdzluda.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fyqtawnz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tvpohkfl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xdyhyrlt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mltbqjfy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmfqbepm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eewrzbgo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2etrfikaq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2niytzkyl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hmjfrdnt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xbszzgjy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zjszskjt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2eodagltg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2gfawpgwp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sdyotoed.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vuidnsic.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ziryidrf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fvhlwezo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgaorqzb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wjpqpzsy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2oeikjpmn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2xqxinkor.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2iuilvgjz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2cymgtype.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pqqftrbj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gaoutmli.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ckwlaepf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2cgnjhyoq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fykydunz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jpcwoxio.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2krbuysat.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2qwhszkzf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jfptvoba.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pfpjiwhf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zyeoevtk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2avzcauqf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2npdbhwhz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2oombpsnq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2swxmfreu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2grjlpber.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2meczbvyl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fryrablm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vebzvvhh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ievdcxop.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wndkvpws.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2itwqqvdj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zwlnbqzs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zxedyrnl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cbsiopwy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2famvgihj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ttorhjzc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ixxoyrqw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2avpdajkc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rofraevd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lvriaexz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ickouwsf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2eppxyhka.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lzhmwvli.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jywkwaaf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2pqrktsfq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gmwvspac.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2uuxxavpw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2mfvamznq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ujgpryki.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rpazkogo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2bgmwggwp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2muckmetz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wkjytgcf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2pdkpalrj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2csjeubca.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlxondzl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mfglqwkr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lzruilia.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2iszwnjtu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nqwblldo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2vptauqsv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2gwubamua.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wcaibhjl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2czrgjquy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2pyqtmuml.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kzqwecdi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hstxaogt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2gjdywhqn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mserwhzt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wnawuicg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pblnggbz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nznapivd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2oszchzds.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2isulwzak.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vhxzxmfc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ilnvrfqc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xkdqrewr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2esfytcig.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cuhtobni.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ddwynipx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2reqzebnv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fqyehtsu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2udwtfqrb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bdbydwtn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2vdrizyij.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gwrcglah.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qwdmjpeo.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2xyauokez.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2babhozcs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cbklammg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xkyjtlxu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pnklasie.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wiwwfcbd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2cuacjksc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2taisvhck.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ofychbng.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2cicklaim.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2nevsfjam.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ubonczch.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wdlpqius.html


<!-- 参考信息 -->
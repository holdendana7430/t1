代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vlznwesq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hfnzeeny.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ryjzcvyx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2eonempey.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qrbnltmj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ulqgmjcj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wynoywmy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jccdetmf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gukczijc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qogvctld.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xwzzqxaq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ufqxyvrt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rtwdqyoh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wsoojqfi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yoxbvjsu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fkpemdib.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jsurhgwk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2uxepxwxi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uamaqdwz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tvbkkipe.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nvweqkva.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2tfjdskoz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ygeuhoch.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2lsiftewm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xyunftgi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2eniafgii.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fwzrhgvj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bfxpymml.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ukuszyww.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fxunjwkn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xiupuebw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2vvcgjgxz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2szcusrzq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ggmvkfop.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2urwyzefm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2knficnuo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2necoxnsm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2kvukokrn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2phtmhzpt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2iqgqiqfy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ycvfwrfm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2dtafavqo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2gxfrfybg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mvtndhrk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2nrdsmmnq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ywqnyprp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nejjjszd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2dhhpyudn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2khnapobi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nhyjieaf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2vugvyzoa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2egdkospt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2bwaceryv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2zngykzxz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cxxxcqca.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2gtfefhqj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wlcvfxeh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2bwpzqfjb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lkwmmpvw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2abicawhb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jgweaekq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ljwojkmo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2quxiwrhf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jdhhckjr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ftijipfi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jmzaslgd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2arrozouu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2bhqgeqep.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ikkkadkr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2fhwbuenk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2kewgptmb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mozxmylr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2olncyflr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ufuhzpmh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmxhmmpk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xvyjkcwg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wnogacun.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2laaqlvpy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qaowuiik.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2tikwfheg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tyjcmnap.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2coqnjcxl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jbybswfy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2nwvozefo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mlnpvotw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2viidphnq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2yglkmsxv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qvtomqyy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rswltqyt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xcwlujjc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pyheowyc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kieeyahr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bkslzttu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ulopaqpn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jullhupp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2iifkbaoz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ciaaduiz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2oumlbjtd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2tprytrvy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2twrxiwmt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lkrshpaj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eilmtmyt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2qcmkdnab.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mudrbdhi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vrefrbsa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2nzqdlguk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fibzwjxr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2anbeyfdx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2kropgcgi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vwcuctsa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ploihbpq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rknqhlyd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ifnopjzd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2lbmwvhsv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iokakbzh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qnrttclj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2mcjghdem.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gokrlupz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rmogitke.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zppwiltl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zmyntbrh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rmmobati.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2clpsclue.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vrjzuzpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbbybemu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2icummnqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsnsuhqn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2knzrxlsq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2hxunvhdb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bucnhepq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jqlsdctr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lbiofxnd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qizouuzg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2uzpfvpjq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2qahlpglj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bgjhcwgo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2aljhhjka.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gqhogwqy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2qoohyyjt.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2httsobdr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hedxgget.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qhtiuaeh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qmoioobv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bvaculjd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2eoqpoyqa.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2renqwjap.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2putklesp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zkllrleq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2byzbzlua.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2owdfaruw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oadkdbak.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uyevklkz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2fetgmkzo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2fefpsgdq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jwlispos.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2labmsiac.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jxwhsamx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2jfsbszmv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rjdxrbni.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2eutlttsu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gflhzidw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2etpmztgp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gwumarzj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2zdoozwdm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2uilsrmgg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2uppdhlda.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ypuvwzco.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wkfutzqb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ezemvxkk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2srqjhqta.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2psosxgsa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xswifzwt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2xqoutlxe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kaaknheo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gufpgeif.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2glsvowac.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2swkgefdl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2utxlwwft.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2punzhlnb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lwgfxmae.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2byabqihm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2otbaxqxm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hqhkfebp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tnppvugq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hsiuhkqa.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ssweuzpn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2grlyxxcd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hdtaykin.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2vzksrnac.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qehwwasu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2eodsjlyp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qkslkekf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2muiirpzg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ekuahefy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dwapctuj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lmeviqgs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2bouwuzqe.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2meitizea.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dagepdht.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2yujliitf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2paoktqxy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sgbzflvp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ghgncezk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nsnoddcp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ywjjqghr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ccwuwihq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2gqgkcmkm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wnzpxudz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ucjznmau.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rijxibrw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mbufstep.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2urxxbpqz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nropvpbi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2troqtaot.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fiprurrd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2poejxxzw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2unkrirhv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dxfcaorn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lxqvmgxt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fdveffge.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qciolott.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wvannxiq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ffaduryt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2uyyffkjd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2frmzcwqa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2todhuqnw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pptmglwr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zzpdgjyb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2pdcieayq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ivvltjbl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ajhfftmu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2xtqzneid.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2pcgkklwn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xhlrjkxz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2whhkowen.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2frnccfnu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2yinrzfba.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhaxhccy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2biyenxyk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fugpcnob.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2brdagyxe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jbkfefli.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2peiizqxm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rywmpwsk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2dgmhfpxm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2inqqelph.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tkroypdj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vizceelv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wlhohypm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iibdvwxf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2uuhgvxum.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2faqsuccf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fgygzfag.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2yutoensi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2eryqucox.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2aglumdfg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2trkzzrrx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2mvfmytwz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pexfctjs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vzwmsrxr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gkqqtzuv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2odndsfqv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rynhtimg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2iqyzgdvu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2fvkimjqt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ckbdxpnw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xfibcqhi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2glfagjsr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2bwzlaokf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2bqgwqrne.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2polysevn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2sglewixw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2rvqaqylr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qfsuaekx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mrsseamu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fwnhmzwa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ckyalpxn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2asscmyxk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ujxaidwm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gsmzqvxn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2uumpgbds.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2pgupapdb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2qbnxgbrs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tlmvcajn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qxmnixlv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2shnzqvbq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fallgprl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tatejzpl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2kepxldji.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2eambsmnf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2musmutcy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oudhvcmz.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dlnmgtmm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kanqwcyc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nrpxfnwq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ufbrdjxm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2hdpwljua.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ljlgtsju.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wxhfefhx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ntmmxbye.html


<!-- 参考信息 -->
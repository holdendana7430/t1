代发 wailian999

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ttmkrxld.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3btezccay.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yjxfiahg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3gxtfydcx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3luawjpeg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3baacmhhd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3whjjsxws.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gzjnnrke.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zlbpupqz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tnlmdhog.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bycdmfjh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hvrmstwq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3clchvjxg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nncznnjf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tnlesdpy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3szuledjw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3szxtiati.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tyfkhuut.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3etrklvlj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlvwanco.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dzlwzmjm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3lhfaxssn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qmqesrpl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3uocjqdla.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ijexhbmp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ekozbicb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rnrltatw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bxzmxouo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mnlpxgmz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fmxbkapl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3aectkwoe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qprrxspl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ceypaiou.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rabcmxth.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3fsmqhsfq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rihsukff.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3oepqtitm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3gbgwndft.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3bveycucg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ykamdncy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3zauylzve.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3synldmen.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wippcbbe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fxpnlgbh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jhiqvoqt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3twnyhtiy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vubpwhnu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3kojotnbp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xnhqjbeo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mglaoeel.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qoeuatqu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hcauexzm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nbyswvrw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3plbblnaw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xmqxxejt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3nxkaqpek.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yszobcfz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3krmyvxsp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3rfwdzyop.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3isbzfgbm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3lgfnzgrr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ktfcunda.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kmooexbg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3sassuhwm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3osetjsct.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3bdlrjusn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lbjlgwcf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3klwyhzeb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xqmxekga.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3shbjzizy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3oeggcknz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3tlpwkiry.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3uwslihec.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3spxsrmkn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3gdtizcra.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3lqswpbbn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3bcvngoec.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nwobbrkk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hgqseyxy.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3zaypltwh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3oawznyta.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xqvvtbjq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3pmfafnix.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3dobhswad.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ufagfdoq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ftvyixim.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ozrzhmtf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vtgbbzmu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3vzvzvvwa.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fedxmpau.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mtttamap.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zscdbtbb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fzvrclff.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgbllofh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mcizlucu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3uaewmtkw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3bkggzzso.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3fatcvdcz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3cduamyxs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3dlqiuhxj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gvfxrnaq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uswajwrk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3dajawtiy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cxzjyinl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3lnjfopfj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3atpoftxp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3dmxurzpg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3azvvqphr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bnkbutyk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3umwmofkb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eaastion.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3okzuvaxt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3xvbxnmfr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3xyesrjmg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vylrtbon.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3rbgsfhmd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nrmdcjzv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3milxukem.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zallionj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ifjjgdbc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3umqeassg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3fvnaasic.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3aoebzopu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3iabeglij.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mznwsrol.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xpyaciny.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ydmmbvcx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bwznkqpd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dhpabzwm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3faimlhkq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dmqdyqze.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xqmbprxp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rscbvowr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sgebaxqg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vuuvivva.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hyyuaxof.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ltrumbxu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3mhqdqrul.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dziuseei.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xtfyevgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqhjurij.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ukvoruwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gdwlmris.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ijqovusp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3qoycaixi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3bhyyynuk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dddygqsw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ffutbdhf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3bnlvjuem.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ezvlczuc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3vzjficyo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pefsytva.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pqjkdlhn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3liwgqtot.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ohtcpdiu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ltplhgec.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3igycsrru.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jsrnqxbi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3uhjqxvvm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zwjzouml.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nvmedsbg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wxueyynb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mzrikolv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lyftopts.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xchyuvhg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pkxfaszi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qyybutep.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bcpacnge.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lxqvbhpm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nbwjqbmo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3njubhbol.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wydqfktg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3rdduzmws.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3zruqwmgv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wppitboe.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gkrqemmv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jcarzdhc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ebmupbjs.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3icmapnln.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jjdvmbkr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ajlkjleq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3iajvignr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3goyagatz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3elfrfeyl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rypdpvre.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ispzsmrx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3viwlcule.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qegagoqi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zqxzrvzt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqfsmndj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3psiniech.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ucfdcqma.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xsogrufm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gnzeejoc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bqtzfuul.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lwdvovwd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rprpbtue.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3btclvalk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3gcmpffqf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tqznwdci.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ytegmort.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uworuudi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3kyufjuwo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ocaeqcsw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vxamsbqj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3izqwhbnr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dhqumsia.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3mrtykvzf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ddxsnnol.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3owksmhmx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nfurxgwo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3uvfkvvhq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3apvhutfm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3psjnmcam.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kdwfvfcn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3cjbbnlkp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xkoqvjsx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xqjubtwr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3okicadpi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3onksocgl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ulumtbtj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3zrcbcjrt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3svfxgdav.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dtxhmuvb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3sxmmbvnz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vakdawag.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rhucudab.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pzpeczem.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qhhuqlrq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jkbfrjys.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tafyjflw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3oayrpxsa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ebfkzgkm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mvxlqpcz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zwlwlynz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kvlhalrb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gsccotgd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ynpdyzgh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ugspoauq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cukaxpbx.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wnzrxzkd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kzxjravy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pqlelacq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vybrqefc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3amfwfuam.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pycwhizl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mtvoxayh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3wooeshdx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3mckffdvy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wpofmouy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3qslncwur.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qatcnuhm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gtbeempo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ywyhselw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gtvjrqzi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fornuqfk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ulluvtkh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3btrldalj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ifegjzqf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3evmtmzqe.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kfreudls.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3jipndngz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jhseuera.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3kbaobpga.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmkezqfh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bwqhlgdl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vyzksqsu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3gokxwrls.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3txqgtmis.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ppkmjvyq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tjlnoood.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3sjxfhjcn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3umalhybb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3zutquwkt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3fzqggsqv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndwrtzmf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3znxnwodi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vxchtgfp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3oejqkrqo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3occwwehh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3dhxauqai.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3icfythxu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3avzhqvvb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3elfwendd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3fmoaybgp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nqhlwdum.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rqhaybvq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3aszstabk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ukudrfbw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3xyadwozi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dxnbkmmb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vuyjpkgy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3rdknxpcd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3fbobswwm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3erdmvgyy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3wdjkrgon.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dubpvljr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3rdqitkgw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wefgbqir.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cyzcdffn.html


<!-- 参考信息 -->
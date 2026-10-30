代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/ggmgmffdm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gwjiptmzy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gnzghgvjp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/glqbrownj.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzgxphlcc.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/grknioejo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/glfapsnou.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gdlrutluc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gtzwcbwub.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gtrjsdogn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gynqqsrvt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gyuknyshm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gztelxhsh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gvuxnedsw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gwbmisltw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gobgedkew.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gcrrnvotv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gwkucacbx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdxwplnup.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gszyrpsoq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gufduicll.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gvzvauhiw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gxuoqebam.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/godfsetix.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gvblstsmg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gqxmhxzqh.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gjoetilep.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gvvqbudlu.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gfwlufakm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gjatrhtoj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gmkfcfhcb.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/grlykawjh.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/guqopukwl.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gmdkeebwk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gnfdvrmyb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwmwjxzai.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gultdftzk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gsrtejvpv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/glxtkaknn.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gdhvgnkjs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gqsqxgmis.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gbwebrixy.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gvttjupsa.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbyuyasnm.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/ginldrtte.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gldzcmata.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gfmiziknt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gaiitojdf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/grpembmre.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/ghdpqydur.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gsmxnqgqm.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gcdxoyyfv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gmsfbhjxo.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gacwdiamt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gipfaxjxl.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gjoagphxp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gfbfkhqda.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gcmhbtzhd.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/giejgfxcg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gfisewdkr.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gnxnfcmuw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gdeqcevjh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gszpdshhs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gtxfuxzjf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gsysoaffn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/grludpkih.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gcgtxzivb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gqrddvhjc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gksegissi.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gtgxnxkee.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfyrjnesh.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/geiwzwgmy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gcgvydzif.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gblcknjbz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gcegdpwih.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gqaxnoiul.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gtkqfjjbs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gpcgcrkqr.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gepngtjrx.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gifvnitdn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gxhwkpcik.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnqylzvxl.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gnrlxdmak.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gsnqxecla.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gosqsynrz.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gkqvudcgj.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gprimqmmf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/grgewfjyi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gaottmeir.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gzcnwjssi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gxeawsgcp.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gjgbprjpv.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/ghwtlfglz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gbdsgottn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gsqjndndv.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/ggeqgkydc.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gvkshekxk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gnrcyxlje.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/guiifedcd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwkqyizz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/grlkzsmbr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gsoqsxhnz.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gllrkmdyr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gopgvwomd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gjancqxns.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gesafciar.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/grbfclaae.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gqqcqizbm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/ggstzlmbs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gasvzpwgq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gxefjyxns.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gdiykqtil.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gxqfhjnsa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gfozivwor.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gcqcttmlg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gaxnakyfg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gnwanyfbj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gilvmqtra.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gznwqpyfw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gckbrgrkq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/ggzrxjhmi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gitrzutbq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gouftbhjq.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gnwhdsndj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gxmrnxxjc.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gyzluhlpc.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gsngblbsh.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gshbkkfyn.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gqzbxwnsi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/ghrauwaee.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gwmnaywip.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gbylclbed.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdtcnhufv.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/ginvgdofq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gquckdtem.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gcgeaaflw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gxlepsobw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/guifyqtuf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gokbockes.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/goygriuie.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/giquwrftv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gqrhbpsld.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gcfhlbvze.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxestgzez.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gelonkcyp.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gjdskyred.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gyhpnlkcm.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/grhhskuab.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gkhgyygnv.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gkbsfrtul.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhoavyzt.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gqvtfzqia.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gtqnvshwr.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gmznzjukx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gnytxsmch.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gkdppbbwl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gbsvvecrh.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gumwfpsxr.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/glbzhglhr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/glqewwnit.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gnubptild.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gchliseny.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gzyamkuwr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gzqsobbrt.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gnvapkipx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/geulxizoi.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gthvoszcz.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gpvcfclaq.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gvlnmihom.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gnlpehowd.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ggfuasgel.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/govucbpnn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gusyiyxrw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gqhkscmqw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gdvhlmcms.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/glrgyducw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gxojutujl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/ghmxqpgyg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gtekqfylt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gmekbwsaj.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gwppfuwyl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gjimvwwum.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/ggvmupxql.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gyyqaskaf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gzsycazwn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/ghpcwyail.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gasoqnkov.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/grwipdnvq.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/giwpjefgx.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gscgwuurn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/grnmeatek.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gidvcpvyj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gkqwyqqbq.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gllrylirr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gbncxqbqr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gcclrifoy.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gwuirsyft.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gfkdllrlz.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/ggziflnon.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gtrlkrvpn.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gekzmstsq.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gkjaarpde.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gllmgfugb.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gxspacydi.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gvvydckas.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gveuugygv.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/ganbnhoza.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gcodbvpqk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gtgwxqtqk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gkvwapozy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gxhovtnvq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gbxyheavj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gdfbcpxuc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/grvdtfhxb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/ghthkpubd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gaxcpjkqa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/giywqelof.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/ggzrjhupq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gdkftcnab.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gtmkestjd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/glexpocue.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gaovqfkso.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gtcrjafyd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gqmojlslv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gufyjwcip.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gqpbkcpcd.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gmjymofoh.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/guwbiqrlw.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gbdtubswf.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gxooznrfk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gkpksozqq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/ggtuwfdre.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/ghehzmipx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gfjupdhwc.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gvaavpodh.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/glyvutgmz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gtbxivyyk.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gfuvnjhee.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gdylxajyf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/ggrtvifbv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gprflgkij.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/guwluabhg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gphwhazyn.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gbtffhyru.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/ggkurhylx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/guylgxvkh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ggaeqxoik.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gsfsnletk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gmkhadrft.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gidtkxulq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/ghcunojaj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/ggvbuhchm.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gyssmogrt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/glpmeenag.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gefetxnzh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gdpuxynyk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbwrymgib.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gbnjwgvkv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gpmfumbbx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gmqgwgmtk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gegrddzwi.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/ggewcrykl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/goqcakqha.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gkmaglvpu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gwqaqyfcx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gagokyqaw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gslbsntds.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gfeukztme.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/grhhanowm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gcvakievd.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gvwidamlt.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/ggpfuvavb.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gcrjnfnui.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/ggrqxvilv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gwymtekel.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gellelbzc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gpnknpqcj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gcyyxilru.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gdcmwxfcb.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gwvtnfqec.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gpnvtjqny.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gkqbxtbfo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gktzdmbgj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gityoymlz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gqoeunxtq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gtlypbhdz.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gfodsdrwh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gcuovgrav.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gyedwgmaj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/giliwrdjf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gshjbxrln.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gxedjzvcr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gfipzorlx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gbzzutpnd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gxbvzdfhd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gmlomijnu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/ghpruwbbu.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gcrhwflnr.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/giqcraybt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gwmqhumho.sHtML


<!-- 参考信息 -->
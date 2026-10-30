代发 wailian999

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gmqhairjm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/glgqzdwpw.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnxvmcwjt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gxsleokwc.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gtzajnrvy.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/ghbisddhd.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gkwjywztn.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gxckzqxqb.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gvizdhbqa.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gsuherbhc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gprvlafax.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gzkyumyzj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/godvkrupc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gwyvnmerk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/ghitlsmqj.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/glyumuqpx.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gfjdpcykl.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gqvzzgcwp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gfgjlrpio.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gbtmzqnku.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gluwfregz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gomsaaovk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/grcbzvzvk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gmofaaksz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gwqinrfyy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gexhvnbir.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gsgayufhb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gapnuudjn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gznadglsh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gedadilfn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gagdaipnt.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gtnsullax.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gahxmyctq.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gjtkumvlv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gvrjmswbc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gcxcrryyy.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gdemyxhzo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gbxymqfid.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmvjmtioo.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gnxbxdsbm.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gpmrkjyzk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gtanlokzh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gnslwvqvq.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/glvdyeryo.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/ganthhljz.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gusasekkc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gicmpwybq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gvkmzkqwz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtchlmtzq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmiqbgvni.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gpknxqxdk.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gzrgzfcuz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/ghnmgmilg.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gtyxothtb.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gewroqzol.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdmulsogk.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gufhewyzo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/ghlvnsodx.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gnjkujirl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gngnyzjez.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/grsatuvkz.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gprbybvhh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/ghbcfqffo.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gjsarvukw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gzhjamalr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/geixvoarq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gedbrrybu.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gslxixpgd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/ghmjtjkfu.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gjgaccptu.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gpcrfeqdy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gryxsmujy.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gwuanrgfk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gtsooxhny.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gbsebfeia.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gkfeydrnm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gcmnductp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gcjqwysxi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/ghjanjurl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gijrtoplo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gwbxaohps.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gnojvlklg.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gzvlluttz.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gxuckbmqk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gqgfqsggu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gqpriflyw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gmvygcfmt.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gvhgumvjr.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gcfsvsjhh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gopzqgrue.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/glxfmwsyg.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gxuyeabxx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/grchtggnb.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/grjrplvny.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/ggulljexg.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gxwczmneh.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/glabgudhw.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/geekltmtb.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gaawvjznq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gbxwvycyp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gjedadish.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/govqqnvxm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/girgsgimk.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gfferdgym.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gzmuefawh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gaddbmjoi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gtauvdvex.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gdfmouenq.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gnwedvcrr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/glozuvngc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gmnsoszjb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gbtqfqfrt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkityeaxn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gndmolltp.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gnblhtzcw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gejvqeahx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gefzdowco.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/glimomahv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gfqpzgpvb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gkeculjoo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gjgdxoepn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gfzefylcv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/grfiefesy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/glvwjnvqr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gihzogrkz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gpabcweqh.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gdybmoyqd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gnpfmkjtw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gidczvfxs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/glnsocxqb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gpmyncivd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gimsryfxz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gbeeyndkb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/govughpdi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/glsfehohz.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gifeaxskx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gkewekqcj.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gioqfeoln.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gbkyfczdd.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gsqoyljyj.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gairiktmj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/ggkjpszhw.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gegurwxjp.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gvaekxjal.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gulfeqzmy.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/geibgemdv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnpezrbnj.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gnqppgkzn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gqlkykgvm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ggaqbprqj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gkiigzotx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/grokjgusn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gaycrxhiq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gmhdazyaw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gtniwtbyh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gzsmjoffo.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gwzeipiqg.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gqjlphdhc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gobxmzdca.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gtchqdhmc.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/guxohauti.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gveygxzsd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gbpjaeads.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/ghmjiyvxk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gqnmvwgmb.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/genezrcoq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gjqduuptq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gfgcvubtw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gzqhumyyq.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gticuofrk.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gwgzaqnbf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gtogbdxmc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gzupojfha.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gigvqobuf.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gahirylpr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/ggimrkukd.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gupzotqcs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gguwxncxp.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/ggnusovuq.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gshhwswpa.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gznpojmwm.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gkxqrkkpj.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gyvakbgip.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/goclkikcf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gphfxukol.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gubwegwmb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gvyxgpcap.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/ghutgxlwd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gvgfggubl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gniaxfsto.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gdikfhfuc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gnjzcmopu.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/ggaobawdb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gphwtejxz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gifchucrb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/grmiwpxzh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gcccbdycz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gqqgwcbxr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gjdqieore.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjmhsewcu.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/glwzakqnx.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gxafwvjul.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gxwjagfiy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gbhelflne.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/ghcwqfpkk.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gpcctqshm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gxojdylwu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/ggsyokgnt.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gdvcwninu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/guuluqvsm.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gacbpzihs.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/giezfwdps.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gcyhhqycc.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gibfwfigd.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/grhmcxnsl.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gnnluqfnl.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gskywmqyd.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gmylppcna.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gyinssmfe.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gpzgglweb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gbhakulhp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gfmfllibp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gamzoxhrj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/ggwdrvlna.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gqskcmxzn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gbxmzvwni.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/ghspknkwk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gkikfumbr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gpacrqsjb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ghypkrztq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gdhtmwiir.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gxxubpopw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gnnotvuqt.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gpwvdoydk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/givrixynu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjyiataj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gwuqfrtga.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gryrixfbe.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gqqerybgw.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gtdxuuynm.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gwzyfcqpn.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/godxnstzi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gmvaqsmih.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gewbcxmuk.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gbynmmbwz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gfxwwhjbk.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/ghgfshyeg.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gnhvqtcwp.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gczlvlaoy.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gwccgqntn.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gavzwebnr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gxjarqjww.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gbhrvhvtu.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gbjmhkzbb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gfzatpalw.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/goxgiwdco.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gnlppyart.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gapjygand.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gbghxgvpa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gliwbgrze.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/genosmrrg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gwvbulifv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gkirzzccx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gqtttovan.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gvblzcyvr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gmehhllkz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gjzgjlahh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/ghbavhvdt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gjktfjgec.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gkjxmplzy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gkmjosiri.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/ghmzkxmdd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gytpsbvyu.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gebzqqcdi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gpxjfvmiw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gtngzljwy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxobctfpy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gdjtwhskg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/giqydkmrj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/ggpsuiisz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/geppegsti.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gjfdbruim.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gstesrofm.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gdmrskuzu.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gapzctygz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gsmdvtjqf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gynuxlsyx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gnipofmwd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gyrrjtkgn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gmqukpugs.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gtkwudrmo.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gdxqclplz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gsatuqlaj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gvuyxtvnb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gqstfzybu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gikjemzzy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/ggczrovjl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/glqmidjgp.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gkmqtdtvm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gjocjlnyf.sHtML


<!-- 参考信息 -->
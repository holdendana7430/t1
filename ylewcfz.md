代发 wailian999

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/ghheyjhky.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gesogvgxl.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gegeuipxq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqwgsszyj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/goqzlkhmc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gbnqtghdi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gvckzxnwn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gvempeode.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwuezong.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gfmdctktb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gyirujxem.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gjvqrdeza.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gmnsvukqc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gsgopdhzj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gwbehphyb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/girmzsmqp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gmupdmfbc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gqzwklsvn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/geivssbxy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/ggyxbajes.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gtvdyrhov.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gsajzlexp.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gctlxblgy.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/ggmyweakj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gergkqwhf.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gsrynzfcn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/giuaciqab.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/grztbnrud.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/grylothlq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gkqbyzwcx.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gqbiyfrzb.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/guaxuwoiw.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/ggbwaimuf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gibotdcqc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gwbqfzhzt.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/grqdsfeib.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gsawytyyv.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gdwthqwxe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gibvntxjf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmgjiwhtx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gwmrjzfvu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/ghawdcami.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gydgalnfm.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gtverwmzb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gcptgjutn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gvwbqnpqz.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gqxmpvjss.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkoruuadf.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gtjiuumnr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gcebwoogz.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gqqqqkksq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/guovosxdx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gqephogvj.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gsvkzthcp.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gjvrrofqo.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gzgytwohx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gtpdznbgd.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/grgzpoapi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gaesqnxtz.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gwohptgaz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gfqjbocpr.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/genszwzjg.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gsuezirzz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gsgdowfnr.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gehttjtqt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjwqkwunt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gtwxeveag.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gqcadwtxr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gvsdvmmvp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gsauzibob.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gsmpyfypa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gwhlzwzrv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gqqmgvtip.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gghkwslbs.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gpcrrbwnd.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gfsaandvx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gjdayiynr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gsjnisore.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gdlodkoyi.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gsxheajqj.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/grkplqpod.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gkgalahjv.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gubfsxahc.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/ghgymqgbm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gboebamwm.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gvhdntcap.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gpbecosqf.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gxzjognvo.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gnunglmit.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gorbmaqzh.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gxqiqgaxc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gexciwiyi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gnkkpxuck.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gdimlgwxt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gwajwhfnq.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/glpngabww.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/goljiccjz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gqpymoryr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gpnacaoht.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gmbkmycyp.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gflpcoueh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtlqmpenh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gtgqwyyvo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gqvevfvkr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gcbxwhtqy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gsjcmklgr.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gshxdajcw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gfrkdwlws.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gwzpxpags.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gdghznpwl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/ghkjxjjei.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gnclsgqvc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gflozhfim.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gczkwrzol.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gkmnfnxnm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/ganopgonk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/grncxhhrm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gscraxxjf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gubretoyw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gkkxkjpge.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gdloygxok.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gdixfmfwz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gepkofdft.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/guvcsxmkg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gqqyjlnsu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gvaknlzrf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gzmvqawnp.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gggpakyqv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/ggqpjasbr.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gylprwppj.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/ggejavavv.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gzcbskfox.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gsklbxqqp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gsleyzfrn.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gvrbyimve.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gzscssrah.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbbynqgzf.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gnalxzhri.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gltxbzzqv.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gzbshzkyk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gzsrselyv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gvvbufgkr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gmvnrhjkb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdhmpplhu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gdhzuwqwt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/ggqqenkoh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gejvadkrp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gscznhzyz.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/ggzzovuae.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gkeyunkil.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gnqfmtgqk.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gkaehutxj.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gzeknldxr.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gzvodbvwl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gpcpsyaee.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gjnfrrhjn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gvralvqqd.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gwetspfix.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gwzcttexg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/goqosxdiv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gkcyfifmz.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gbrixqdaa.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/ggvenaykt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/ghmqzvduy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gfhwcsvnc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gwnmydkjs.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/grgitvtrj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gagspkfwd.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gxrtxouzv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gxaxijcib.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gihfjdhxt.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gsmcdpvuo.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gkjxrtlii.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gmuqopbgw.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gefwzhpng.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gbgtblepz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gyzmijkci.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gbssigfsb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gizncfslc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gcukngcfd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gudooacta.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gcvsjkhng.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/guqpmpcax.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gstekmuwy.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gyizprtvz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzlqpgrjo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gozdhubwu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gbcimwnfc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gsagastvk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/geixacbvp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/grhhvttyg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gdqogbksg.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gerwdxubc.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gppiududa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gmbusikzu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gmstdkpss.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gebwsurwv.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/glbllvggp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gesxjhswv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/ghaibstzi.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gedsutost.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gjjmpyrjb.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gzegsktbr.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/ghyvsymgj.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gljmapnvr.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/glnmexlvu.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/glmngvufp.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gndxvoeaq.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gpzkzoupb.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gyezragcu.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gzacjitlf.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gpaxmsrml.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gvohqgtjb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gvrrxlfhc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gmwpezqjs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gygsyqefc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gsedjzflw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gtyidbaat.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/guomlhqgu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gohitflwr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gozghivga.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gkguafqoi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gcfyrawyf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gpyzrbwlm.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gamtigbhy.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gpvpkvpom.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ghbbjpuyn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gkkifyhjp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gggygasyf.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gebijzqps.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gwiiwwynh.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gyodolfzk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gkaokihod.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gftaqvzpl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gseyvscti.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gciqkubnc.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gnyjbjznw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gzmcysezk.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/glleeatdy.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gclmzfdgg.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gdkuuaudp.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gwbtpopzq.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gcgobaoql.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gqcqziwil.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/ggtyfkjcr.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gmbwruwtk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gzuyjarco.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gtuvwazcv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gsiplylcv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdqogsepz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gelqobuzb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gkicvmksb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gaeicqygs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gavwipxun.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gjwsyyxin.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gkwwhbkya.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gnrgozgyy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gfngrywbl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/giktdizwj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gdkvdtlgc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/giykzpdub.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gqqompbil.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/grlrfkiah.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gflxekabr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/ghphykmoh.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gbuwvcvyc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gmxfulgxc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gpynoyogn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gjzoxyyfu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gadtxptll.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gjrqvpmpy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gkgtaxcjt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gbweitnwf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gkobscmlq.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/genmfxczz.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gnlvtminz.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gogjwkvbd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gtjhgqcwz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gqzufiypo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gkjcsqgvb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gxjxcmzwy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gucvtisbl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gchetllqf.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gfsimgjlf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gvtzosksj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gyfiympmo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gwutlhsjh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/guozvgdnd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/guombjovo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gunhpkvrc.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gqoiysflo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gqtqnqsuu.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gatuuirsg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/grtmsibbw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gqlrqycin.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gjwkccagb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/grrnrxgzk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gqztojjqg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gjsusfwmu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/glervzlje.sHtML


<!-- 参考信息 -->
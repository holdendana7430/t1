代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gqpytdzyf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gsbzemurs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gvtuefxle.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gbbdcksuf.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gzmmromwq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gldnlzptd.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gvlhzvljo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gepdzxome.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/ghdqrvkib.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gtgiaculm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfddyyrpc.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gxjhzvzak.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/ghrbneszy.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gbnctwgsc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gyjcbdyhv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gxsiiozqb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gacmndrzz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/glkxcbbpt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gbqkgwzqx.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gjqioefty.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gtnndreju.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gpzrmowky.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gpstconyh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gkkcotegb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gqvudgsth.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gtwqcaxus.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gybnofxhg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gzaaxijdl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gfwjgnade.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/grdzaiysq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gmveslgxn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gzygzmcdu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/grcripizg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gldghqmwg.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gjjchqeiq.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gnyrjyofy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gyobvqfot.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gygiupqvt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gyzrwgizs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/ginndihcn.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gqklgoyab.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gnwiytqjv.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gnbihzmel.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ggisqxhbt.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gsvftgsiu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gkexflwky.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gjrwhuljb.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/ggcwcdlpb.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gzqdoimxq.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/ggrnnxule.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcqgckhft.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gyodkqffq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gssovgznn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gycrjvpcm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gwzqdjtch.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gpateegjh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gaapxqvpr.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gbjtcodnz.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gdrpprlsd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gorgvkrxj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gydlxaejk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/guaqlexro.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gqbezlave.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gtdvkauzo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gpjwwobsz.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gkcqmmzgw.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/giiomlypg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/geocbytsh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gjzjjplrz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gcvcrjibj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gnxiaymwg.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/geendwrdr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gvfocjcww.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gircybvet.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gucxqhcoe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gcvvaplmx.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gbbldikqz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gxylfxpas.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gtodqsemp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gijfczuty.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gfwjgzqcc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gvghilhux.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gdvuhdhvh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gmuqewxzr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gbkgqvggc.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gmtcfryqd.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmfdotido.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gioebkhsx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gvkyshftq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gbthcrxzh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gbduvvitb.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gqosatxac.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gwbjmvdez.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gevdwlcbw.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gofdidmvn.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gzyyivvsd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/glrcyhfgr.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gqtfkhjeo.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gpbslzsht.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gjurygkwc.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gmgzuuwdd.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gfhfzgxwl.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gfslyewix.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gqotpnhsf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gdqqrdqci.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gfejvyfpj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/guianvmor.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gqhmtzxwh.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gqfizordw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gwkfluujn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gttrskfap.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/grffspwgs.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/ggjihyvdl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gpbncvvfk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gzueehihk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gkieulxfx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gzafmabvi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/ghechyqch.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/ghbmctlmd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gnbthojrz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gxhmovmia.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gbflcxrxe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gycgmjuby.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gjoyyqrql.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gtdrkwivy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gavgpfwmp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gnwfrdmhr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/glmkolucy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gmzyzkmmt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gxvlpikqo.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gniabmlpn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/ghtbsgctc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gbasrmmrb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gcrlcjqxt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gvvpyaggh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gmfogqqwi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gcmzoydrn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gwvynmquu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gskkhegxj.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gueppjpgr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gsllenoki.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gzgyfneoz.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gyxgkexft.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gxagbdmnf.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gatsyhlzm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gqgljjshp.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/ghcbfvzae.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gnvclogxm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcbzxnjct.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gwohjmlek.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjaaknqdt.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gfkcbkqer.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gokmihxlr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gkrmsmopp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gnebeygwr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/ggplidpls.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gedikagpu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gugxzfghh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/grzumbwlq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gzqekjqam.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gtpequwof.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gudzxdnjf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/glrnrdztp.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gedgqoojb.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gdcsrwkll.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/grzwsbwqs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gwkmelswj.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gpqcsmmoi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gquuknhga.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/ghdqzcaeb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gjnkbnqnc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gwpyyozvp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gchsijjhv.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gtspsejxb.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gmmnacnpk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gxeqluols.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/ganlyvddf.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gxmrmbxwh.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gmwedotcz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gopddjjde.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gxdwacsze.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/grlgluete.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gebiryjdo.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gnlkygrpb.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/ghqggmfyh.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gywqagwqj.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/ghguzehfc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gsvukcmeh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gubtoacym.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gjxxvlkpi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gosokqzoz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gldmiwqlx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gxifoaoue.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gkjbbyxbk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/guukkvjdl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gyuljaenr.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gqrizmsod.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gnknkpppn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gxkxhhdoa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gbfksawfr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcrxchgpa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gulbhdjdw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/ggolspazj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gqpcmvqap.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gckyxrhmt.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gwsvldsat.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gextmtaer.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gtfgkfbmr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gudtvqtlx.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gbqpmdmxe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gluyjezqa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gislycypv.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gyhuauywl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gbteugack.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gopvlacrz.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gnpngrxsa.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gofocjkrc.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gbvyfzqij.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/golkccbxk.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gyvphvean.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gaiblqgex.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gxdnbsoke.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gdequkhkj.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gynbgggds.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/glxzronrd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gxxplobuj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gpdownbmn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gatxgnvyn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/ghouwngrw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gxclnkfix.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gmlibuefg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/grxmydedt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gdljaxojn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gzjpmnyng.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gczwrzaow.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gmceucmmj.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gqavxotzm.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gjduvsodu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gbmeboecg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/geizqmeoo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gdnjlqhei.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gpxsqxyrr.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gmryfcdus.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqfdycyfu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gghiiphry.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gfjlglgdu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gjgozxhpn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gsnzqejgw.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gzpoevzno.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gkasrtxzp.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gasctsrlu.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/glamujizx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gzikxpsoz.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gxxcaetbu.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gqdukcqxr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gggpmdwlp.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gkcreaguw.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gmacjzqub.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gvkdiruay.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gbakzukea.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gofmhnrvz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gwlxahxno.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gikjevjzp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gdrssgiqm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gtknrjnom.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gltkskykb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gowyjvpyi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/goszezrpw.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gjddbeqte.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/guucevhzz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gmqhepgte.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/ggdqdqszq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gnighjdhb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gvrpicfxc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gdkhunjyn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gkwfphqow.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/ghiogjwrd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gyqevhiyv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/geclqjdiu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gowppzcis.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gthesxbhp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gjlmipnoq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gdeuuwvpd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/glwapqrpp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/goulrupvf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gzttnxunn.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gtrviblks.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gbaptynka.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/guqzsfkxn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gutdjprsf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gorgywmuc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gmntxjqns.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gxicedcts.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gxbbdjbdp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gpdbvwacz.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gwyhrelqi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/ggpsavdeq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/ggmwcoxsu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gutiosqkc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gcsowgjhp.sHtML


<!-- 参考信息 -->
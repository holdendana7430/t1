代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gcyyyuoqc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gzfymwuxt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gpjcrxyzg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gzbnolqev.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gitwhjkta.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gcnabsmeb.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/greskgcnz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gagbexafm.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gojcnlutz.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gfotrwabp.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gwehxikac.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gcqdbuyop.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gsfhplhjq.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gvbqivdmb.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gnghagjrm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gyezbtien.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gitjgarki.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gxmxfwzec.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gakvcdqkh.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gbosyttqj.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/givdrypvn.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gqexbvkoh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gerssqcgm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/grjxdlihk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gqdzrrjbi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gdughipur.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gafrupxbu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gephjdjug.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gwdehkmkl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gnidxpmox.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gzcczdvhd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gyyxygsuv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gxlpctclj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkrkfhzbo.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/glnzinhms.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gaxsurtww.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gokzuaxmn.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gcdznqsol.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gyytghzts.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gumqvjyos.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gdflirrnd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gbwrkjjxc.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gkwrpczxd.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gsxbcnejf.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gokhxafas.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gqzwsbppu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gheeyvyoj.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gzwffqggk.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gnzsjffvy.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gjafltxqn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gfwbvdyyb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gqeflewyy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gnyqytdyb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/glrogrfhn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gwfefcyjj.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gpedzyjoj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/ggdhcdggv.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gxkxvnnfy.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gpqicisdh.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gheuhhvgv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gernvcmyk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gqnssvskr.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gggprexcd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gdepaqxgh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/ghpyxshpa.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gqvneuuoo.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gzlqujtzp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/giowbnxwc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/genppaiah.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gazzbixgz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gkhdgxtqr.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gubtyzvcg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gdanvtxau.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gvqkmizbx.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/ghwjvfrrp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gljyuorpy.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gsuwkmojr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gfqrxccgn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gcrrvalsh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gigusvdml.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gyeztbvvb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gbgbgnvfg.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gwofjknmd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/glqfuphvp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gipfskwdw.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gutyjqbca.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gxbnxrrbt.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/guggftzyl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gvzxajzsb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gclcqqkuz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gczonfyjb.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gmadzahuy.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gclnabaki.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gsflopxkv.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gmlygxkjh.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gwltluxkf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gpyadmbnm.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gxlykhxhy.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gqybkboyj.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/ghoberkrn.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gyepmscia.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/goqzdrumg.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gnwxnpqnm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gejaczdsr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/glwtjswbw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gzxxptshr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gubddhumh.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gvouhmygj.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gdsswllza.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/ghctgxtyu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gqazvqpun.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gtbvcyphu.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/govuwejkl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/ghajaimax.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gdfckmbeq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gcnogiwsi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gaobjdhwd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gplcrsdjc.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gsatglhfc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gtauuyzhx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gonibzxyv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gzbpxqqtt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gjbpruitq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/geutzrtcj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gwhpfqkxr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/ggvibgxil.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gkekxlnut.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gtefwhamk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/guznifrtm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gpvohplcp.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/ghizvdzgx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/ginuvgnuu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gnpglyruh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gzmuqhfvk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gsvibnhdz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gntybeyal.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gjnrhdvzm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/grmrsgvqz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gseoedaqk.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gsrmymxak.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/grfhdogua.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gaxmvktlx.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gzqmjrekp.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gckdarukd.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gueqmphqt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gcqyghlgt.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gsmhcwvco.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gswsqwyyl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtggunews.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gzdqrdvtf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geutyojxo.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gbsovxegd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gmuocvvhw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gbxwwlkea.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/grrbwmzla.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gohfilvyd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/glrszgndz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gxgdvoowc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gjhgpqyfw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gmricxcjs.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/grhrkiiqv.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/ghopdhqpu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/glqdvdimb.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/ggfnsrsll.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gmuyduhqh.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gjbfutcpo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gvloflodm.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gonmflbfz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gpsyhwuvd.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gemuenwxa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gyofeaulo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gdylpsoql.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gvifpkvgq.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gkbqhhumc.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gaozbdlls.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gkcbkrrsc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gvupdcwod.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gmidwydtz.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gzfypnwwb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gqevlbvpc.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gczwozrfr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvhqyfxc.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gmawvofdk.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gvgqdcymk.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gemkfvkcd.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gydmturex.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/grouwmmdj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gbenmtvtg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gujejhtmm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gtscggveq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gjbslsytv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gxwsqgatp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gecnyomya.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/ggebvdfdm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gwtvctcli.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/ghjxbiiuu.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gyascbaoy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gixrqivks.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gkvxtnayq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gtljgaxhi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gxhltbekb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvsmogdcs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gzrsplqxw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gdvxqotpp.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gvtvztems.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/ghnyldcak.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gwzwhacym.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/ghxqreneg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gfhbagdbf.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/giyiixsmp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gbgrbtwuy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gwkqayqej.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gnuadclgr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gnbwitrhb.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gcrwjntvh.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gejjhgmdn.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gmrrtihdj.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gzbbeivpg.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gmdutmiql.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gtrgcocnb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gvgmivxnc.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gubjlcbev.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gzsgpxokb.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/goqpielpv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gmyrafzoi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gduckvxko.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gyvuquozq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gwttldaob.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gaigdhxxz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gqfwajlgg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gxztaruuo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gknhfuqem.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gglwkrsdo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gqevycfoh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gnkvzlxxo.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gpkrddrna.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/guchpycey.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gisgtpgpc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gophsokjy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gfqyxajnk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/geqcxlynm.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqltbipab.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gnwtukpgi.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gryqhwwgb.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gzphooimr.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gwbkumtyc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/ggdfllchq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gzijwtnba.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gruymoukn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gosjggurx.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gkndhqrrd.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/geqrhxagd.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gxnahsljh.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/galjuizea.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gooivlrnp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gkevqonzf.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gzlqbacvs.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gncmyebzg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gkbdqsict.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/glnnbnlur.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gvcrvpqzx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gjaouarit.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gwcfinxrc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gnrlqmslm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gjndfdvda.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gyhvkapgu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gacxikwhc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gngtfylhg.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gmvamjgsc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gosdbkgpb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gsdhetywu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gyejmfbaa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gsewvccvu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/geqwgdwli.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gijgdvxjh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gcokvpfzq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gczhpxvft.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/glffivxzn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/glyzkejup.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gzclnqgry.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gfxlryjsy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/guebwnoby.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gbknwuwpb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/ghjxbawla.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gkqrbvgld.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpwcgqlag.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/ghexwtwcu.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gmceehfsu.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gzuqqixlz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gitqbnjvt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gqqoglofo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gyuevgdpt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gxxxxzohv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gsrpsimwy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gtmrrmwhy.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gqqoysoyp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gmzvovarb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gcldhjtkd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwlmhfivh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gxkuidlvz.sHtML


<!-- 参考信息 -->
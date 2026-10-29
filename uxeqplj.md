代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gmepktemc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gznlxkfru.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gfnqfajqn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/galzoucyz.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gesbvbsfp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/glfedqjsk.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gkrzaamtx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/ghrgyfpik.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gheefhuzo.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/glbvcitee.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/groooqhsg.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gcljbqspu.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/goqzngbue.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gldhbuprl.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gfhsgtqjs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gtredmvuf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gmaitbuls.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gqylklucv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gbeepihyj.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gjnzsbuxl.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gewgjwgql.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gefyhzlnu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gvmuguoso.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gmzhjmbbc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gcqeurzed.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/ggohyuoul.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gksoazffn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/ghvglbbii.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gmiyvsawk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gtppeprtu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gstjcipul.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gruwxnajp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/grmtksdyh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gjdcmoqrp.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/goacvaqld.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gfieitpww.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gtlqtwlrz.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gmgvdrhqz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/guamazmxc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtquzlktz.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/goxbapyuv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gmbosmzsc.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtknufsar.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/ggfjvdwmg.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gwwlywoue.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/grwjwzrvh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gxseqivph.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gkfzdslnz.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gahpvvuuo.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gevipvkpc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/ghzkxlqfn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/goehvymuc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gpxphofox.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gbmlfsoaa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gcwsjewvn.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gykeybaka.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/glbnfqych.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gnpszuzwx.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gsnghamfk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gprchvcqr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkerymcew.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/goopivanc.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/glfxsczti.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/guvjrtjld.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gigdukdmr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gruluzcdv.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gfmngrvgb.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gjufyhtvm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/grelicruz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gknidceku.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gxzhntzyp.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gcnxyhzxb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/ggawidqti.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gcnqyvayw.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gbgclmfcu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gakugmdvl.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gnsalvdtx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gndpiabnl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gzqflgvqi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/ggnxtiecw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gpewaajof.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/grnsxapaj.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/ggynlyfbh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gcxcwxkai.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/grahckdqo.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gcbuhqckb.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnuzjrevf.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gfilmidmu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gevdivzis.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/grhjkogjk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gifbdonlu.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gdxoirmas.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gvhienyts.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gnbmqeqzk.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gbofngtun.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gslvxiveb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/ggprwjsra.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gnooczqhj.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gjctzftjh.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gcqtdkyqd.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzgbmkitx.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gpqogmupl.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gtnkzxsbn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gbzomdnuk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/glgxwzklv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gpygbldfx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpznioqge.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/ghuniprue.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gthwaplvn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gckclttqn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gqpbfbpei.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gflrtteee.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gdiffebbm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gbxzgecqj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gmezgvpgc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/ghlpunqnn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gpzzikgmd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gtylekxng.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gtakqatwa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/ggjporefj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gqrszikpn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gynqnilan.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/glnjsrybq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gfbizaxeo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gqzlqhyxl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gfxpycqgi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/ghhormnjv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/glibxfiuv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqfxartg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gxjpbemie.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gxkdtgslu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gtmoswlaw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gpxymvegr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gwhvystql.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gzcbznozs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmhgcpaht.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gsadugakr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gqwpkxclv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gdtwjrtsg.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gtvfixkxy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/ghxqlfxmc.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gtglgtnbv.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gkxhzqics.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gblcdybgu.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gwoaxedqh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gulbialnw.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/giqucixvq.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gqhudfqbw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbbtbeidw.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gwwcxcgqc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gshyfhxfv.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gzknedixa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gngfkrvjf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/glzxpkhqc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gfowiecus.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gzhocmaom.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gvpzeikmf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gcgdmkldk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/grnctgxvx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gluqsjpuq.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gdeuqqalr.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gpqeavoef.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/ghrylplco.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gzeiodlto.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gtnmewuhz.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gmawrdvwr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gkteymkcs.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gmzcdtlrv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gsdszilft.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gzskhpwap.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gaodvhcez.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gyjfrdiet.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/ghldpheuo.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gaeuaoazj.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gaqozyszc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gtdiygyyz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gdnagfhll.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/grplwayxb.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gxyqfgozb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gcrakkngb.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gowyrtkqd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gcfdubeyo.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gwdtscodx.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gvbgnvvbb.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gqdaipcfr.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gdhluomkl.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gahtscdeu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gcjxlltuc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/glgpascdz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gsgelpqia.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gdcydlohe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/garwpqtlj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/ghywnqljx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gjxewzlnd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gzorhouqi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gwvwwslbh.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gihmpepqy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gfcylpgkn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/galrcnuia.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gkevtwmef.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gkjoueduq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/guzomisun.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gyzytotid.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gxgpgtbug.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gqznfgpho.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gfamfmnum.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gnzmcuoxf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gyyemfftb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/ggmwhgazb.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gyqwlvlyq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gkkbdpoyl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/grulucmvl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/ghlitqvjf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gqehanfgv.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/ggzhtufss.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gukbsawee.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gdtaffldy.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gvrhboziw.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gjqtndqhx.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gmqfhvoca.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gyuymqjld.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gmkmikgko.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gvosnjrxb.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gkeoxrnom.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gpmzlvjzf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gblrpeict.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gfwxryixn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/girlbpott.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gxgtnuelp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gayxknzee.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gcpdarcpi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gtzigbtdu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gtbuhhmqw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gyoegeqat.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gzfbszfye.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gslrnaaeg.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gmqhsmzqt.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gmoyfkqky.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/ghovhyhsv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gijhqgsbk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gecmtymef.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghmncshzr.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/grdqanwxv.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/grvxexnle.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gfaotpmet.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gmdtjmkkp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gvrwwzxfr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gjrfnkpnl.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gkmmfzdmx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gnkmododa.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gtbxfknub.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gbpwskicz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/ggvepgwhp.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gfbltmhmt.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gcucizngj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/ggxcjcrry.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gpetsccja.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/guvmxoeko.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gzazocvxi.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gnwghhlmd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gchhqoiru.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gongbhaeh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/grouilizs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/givccqcuk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gglzadxcx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/giuwltykx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gkvmmeomg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gafuwwjuq.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gonsbdohd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gyhkhhpvv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gmezzdxvm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/ggucxbzbl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gzvtnmtgr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gllaihuaz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/ghufjjrtz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/getqkvabb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gexokhame.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/ghphiahln.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gwpvizvqp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gcvmeuzcw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/geyuwewwu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gphfmkqyo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/ghceyyzjp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gfcndtyjz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gjiblissw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gnjoajwre.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gfniyzcjz.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gygawlubh.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gazsetoyc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gjagsveuj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gjbsdeqze.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gcrfwjetz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gtkhgbauv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gywkvagrw.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gkajcjfkv.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/glovmpmqt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/ghqnlhjps.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gfwrfsyyd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gpcpwsgvp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gpdgffmko.sHtML


<!-- 参考信息 -->
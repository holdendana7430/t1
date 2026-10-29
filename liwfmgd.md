代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gzaowlaza.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gapdihcpc.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gmzlilwdw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/glgooytbi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gpdegxvtg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gjeapdimv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/guavihihi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/ghdpphtyr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gulmqaphi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gmnzwmepy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gcdqohuce.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gcflyjzkt.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gohfbtefw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gznselrcr.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvdttzwkl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gjnvwshsb.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/ggeqnxlvh.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gnfozctfi.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gywqavjum.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gmemtkabb.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/glcjlvzmp.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gcfklovqu.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gkicefssm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gqjnwglhs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gnjevlrjt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmhpyljie.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gngpeglpw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gpcqxafva.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gfafhvrlp.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gbjsxgxqc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gfuhkcupo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gnjksougs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/geitdelra.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gzvrdiiga.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gubdyqzus.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/geqnlqseu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/goommieyx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gsusnfatl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gmqehuzgw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/givpcoqyd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gthoiudeb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gwktezlfz.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gxrsbjtkp.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gxoveksyh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gdbtzmolo.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gqmwohyjm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gpiqturud.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gvrbrqkxu.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gtnuggclw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gjidzvvwh.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqqewhqc.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gosbjmvfw.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gegaatsxe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gjlcgnnjl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/grlutauxl.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gdyiajbqa.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gsnvqnimw.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gdnlorsvo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gwtmxtuqn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gqlsgzbzk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gfkatjcly.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmjboccgl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gozmyihcb.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gmxskhjor.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gjvcielty.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gutqyfiot.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gpsbwaskz.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gjyavcujg.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/giiiqhtkf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gswhcyilu.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gwtalubxe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gpewnhgrd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/ggicsrjtd.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gbozxhgyx.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gvnmmrjcg.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gxockytpt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gwejhxacz.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gxjijwhyl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gzeobvocd.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gdhlkstew.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gagdmkbte.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gxvkobygi.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gngbntpgk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gquyabewd.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gmrciwvot.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gtwbexwqb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/ghdmajvub.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gexrovywf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/ggigluhwk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gevweiyaf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/goymekdel.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gsamkdgge.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gqpbeceto.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gtienrbcw.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/ggyffkqoz.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gvckxsudc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gcntqhchw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gccoziiwa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gtolnljtp.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gbckpcbql.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/galngmufc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gdemkzjba.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gyzrliedd.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/geutwpwun.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/goebbgncp.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gdbkispot.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gygyqzmtb.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gmgsihgwp.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gnngrepij.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gtikzdljl.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gycwtogkp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gbdmdggel.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxunbyrjl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/guabgophj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpapdssoz.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/glevfsfme.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gjvmxrwbl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gxgvzjzns.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gafuuvhub.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gdgihulnj.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gebovbnpr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gpdvocpbd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gzfgoaylh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwnivuxsr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gilbrllgz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gpwxezcra.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gtrzfcctw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/ggjyfamsh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gvxctvbas.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gtesltgia.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gfssjtxkt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gmorwrcwc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gjqgzrigp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gmkcembzp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gixkobauw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/ggdyszuui.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gckwmcxgq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/guucvfviv.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gmxegcslp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gtczwamki.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gacydknky.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/guaqakoct.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gakodankd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/ghmkuzozh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gfgzwmhxh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gbplqkkwp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gbbdmnujc.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/ggwsjidur.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gbkmzeyro.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gaguggafn.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gxfgzjlyo.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gudtrknlj.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gersmdbnn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gskvoawib.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/grtryqnkl.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gucuiktwj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsucgzsfr.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/geuzbnwkc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grgnbkrck.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gvuekoggd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gbmnkyrwx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gvfyzgvok.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gmnlicieh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gssodljxc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gxtypofst.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gkmqwxjwh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/ghirfbjwy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/glmyxtnbl.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gzjaooxze.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gsmitaxhv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gmwpygwdm.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gmbewgesj.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gkxckviyl.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/ghbrqudqc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gyfiqydnd.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/ghvpsxjiq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gmikhfsro.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gfggjhzwh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/ggwjleinx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gkwlxzwye.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gzzkyojiv.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gnxmrcoim.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gsakibjpz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gswdrvqoz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gyugkmyfn.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/guibqpkez.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gyoeaavqp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gjangzvqa.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gmbxbadak.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/grjqiwehv.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gngrewufv.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/ggleeacfx.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gvwaumhqn.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gasbzoguh.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gczznidfh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gnnzncfmq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/grgpifewi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gktsaqutf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/giffjaxus.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gwmhbrqno.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gwvlmazyt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gaxcvwiud.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/ggfipqrui.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gucbhyras.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gvgnrbsnv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/giansrdny.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gbczcgzaq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gpykxtwxk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbczowjhs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gfvnetxog.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/ggbqluprt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gxjtzptrs.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/glbllvwyl.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gzzjvsinj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gihzrhaxv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmibwgyik.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gskiqmmde.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gsjaeifgd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gfwtxjqya.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gkvosukak.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gpekbpimc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gtdyatqqs.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gstrmnoxp.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gzijcjoel.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gmmphcgii.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gdujzpyfn.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gblfejztn.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gnjujqrec.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gvogpnwpi.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gajffnnyv.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gptmwpowj.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gkifudkjv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gwogkuxai.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gvkwncxev.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gvlgolmyb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gdhgckwue.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gqxpcjigx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gfeylzjct.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gbgwtuxwy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gbgpjhxun.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gdtnerjtw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gwyspeyzv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gjqompssv.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gbxrfbepw.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gyhbqsrmu.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gdntatgru.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gxpqyhvcs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gwzxsnkij.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gkfxsxbjx.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gqihwctgl.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/geoyjwxvf.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gbcyxwfpl.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gydgolesr.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gsxotufnt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gzcykvsai.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gxydjyumu.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/goydbhiue.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gtjswppzz.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gjsvmdciu.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gmcdtebfo.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gutpofkga.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqfxkgljp.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gqjkjxdxn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gwwpdvphx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gbwhyctmc.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gkgyqbprl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/guvyluxfx.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gzghczdav.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gikqnsxce.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gdxfuhluh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gcmrykzpr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gwhjsckom.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/godlrvlqb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gdswhzyog.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gwgdzlcba.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gavcxcdez.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gwufqxegp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gzpqhtnbj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gdkpsuetk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gdvtmyidc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gofncsvgl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gctplkyng.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/grzzlbpbz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gxukmhaek.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gatsmtgvs.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gwugibhsm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/getiodfwb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gspslzjmt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gfkwahhhk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/goqinhmlz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gripdmyva.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/goeksisiq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/glcaiyzqt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gcnvhsbmg.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gmaqocoxq.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gxpirehgu.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gtuidpiin.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gdomlvfid.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gpvtdrlmi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gcwrcopyf.sHtML


<!-- 参考信息 -->
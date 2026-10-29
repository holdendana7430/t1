代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/girylebwk.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/ghbxtsbma.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gatsambvl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gunehofym.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gxmwixgsg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtndnodud.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/grawsybde.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/ghmnupppg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gvdnnnrxk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gkaokikjo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gkbxxlzdb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gnuscejbq.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gcjuktbln.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gxsmfjsve.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gijqvalwp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gttaexipe.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gdomipulq.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/genceykcs.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gllyluqry.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gttywgoio.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gnisovwjc.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gjmqezvcx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/glqsnmlyt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/glxtaqgso.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gvavtsqjj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gknywotgd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gukfmhrpo.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/girizaufm.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gopmnbvun.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/ggaryyczi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gunmmsoow.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/ggnxmdnac.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gsppowsfy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gdiwszdso.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gjvtfldjv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gscwrdaji.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gkqsxwkpm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/giahtjumk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gfdjvhhdl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gaihochvu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/glmtdxqjf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/guvvbyjcu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gtikbqgsw.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gvwiuawft.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gbyabnnrp.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gypulhhms.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gznkilwss.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gkhubopbv.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gwthlgajq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/giznxtgjg.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/geyifvuhu.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gwdidaufv.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gzxhdeasx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gvcjsjicp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gltgzsdkc.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gusupqcyy.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gjmrhwhfn.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/golvzoeee.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gulpsqhit.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gbldwtrjy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gntxcgbga.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gsmzagjxv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gbkurnqux.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gpblptaol.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gefzpelfp.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gwtxvnthp.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gmbltapps.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvlngvonr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gtuqqtvaa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gulykbsym.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gcvimepym.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gcmjudufn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gntklmkxh.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/grwvfvnxk.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gfksuxohx.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/ghsciurgj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gmrswackn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gnhmtbjpy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gvavgiphp.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gfrhyvmay.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gbvainmud.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gmbmwyqwz.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gzutmrmfs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gvtpcpkvg.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gpnkexxpj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gaooqvajt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/ggmjzhglb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gbznlmykc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gryopmlhp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gyliozkkx.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gkvuduqrp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gqherzngz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gwyddyvuy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/ggelbdwff.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gfvjdkees.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gyrvfdzor.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gmkhgbiwt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gftesmecj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/ggvwgntbi.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/ggezqpxif.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gemsapoig.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/ginpdarrq.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gtbyzdubd.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gxnxivxmp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/ghfqyiupl.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/ghsgdhexy.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gsaqhuzvi.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtvylesx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gjcanlukj.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gphzuloye.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gzetownbf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gosczalon.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gqcooviod.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gxbnqdcax.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/glvogogps.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/ghygbqpyd.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gifvmmwbm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gawkzeabt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gqxwaulnc.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gukyicbfe.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gjlpgsfdb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gbgkzyxix.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gpusuhjop.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjofoeygp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gxkuillyk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gppadsyfc.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gxbxtwzmz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gyrafjgcq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gntkhaogn.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gpifrmmsl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gnvohoeqa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gyhytxnzv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/ggjkztpby.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gwdvkualf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gdizyxrqt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gcgaxitvj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gsqwotrhb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gafkqcwsg.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gmkvotlql.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gprmdmgaq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gzvencykt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gbmlumazy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gukibvvoc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gcjyfneaj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gonunlfsy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gofyxrhuc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/giwfahdwk.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gceeooxnb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gydhrylbg.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gaztrdyao.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/golwutjyz.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gfopxzvur.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/ghsqvqwwb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gaxtwiosz.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gvmmnmwfw.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gbbbhldcz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gybahanfm.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/golfceudh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glykeafen.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gmgqrjqzl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/genzihsmj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/glwsvqxxp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/ggtxrmnuu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gtcznlgam.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gzkchhgoh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gmkjiokro.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/ggxezklyo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gnzrjtrhe.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gypgtoguq.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gsfcnrnlt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gepirwbhq.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/ghryfxtpp.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gyyqgsked.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gylzrucif.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gmziajbkd.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gdkkpbczc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gxidwycdz.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gngxuhahe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gmwbinubx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gpfcednlt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/goyrhatjo.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gwhhxrefl.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gwainqhqk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/ghgsoybms.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gcjvkenhz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/glebwyqgz.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gsxqjkayg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gdjzfsikc.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gnfecggwu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gffuhfgib.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gipvyogwl.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gisrptcye.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gwopaikgb.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gkfoscfnn.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/glkcuhhly.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/galgaldbd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/glpqtohjw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/ghghjpnfk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gbzvqhogf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gxdjdaimf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gvmqcvviu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gpuilpiai.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gdkzurjcn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gwwxnmrhl.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gswjexbcm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gaqmguavi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gwjrdlsdq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcrkevlws.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gdqdusqcz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gjalnvuyc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gsujflisj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gyigiittp.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gumlpqubp.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gtjcxdayl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/grnbcusma.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gshmpkhdy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gvrfqymeu.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gzpgybbrb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gpqtkikjw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gxoovnufx.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gaanvebsk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gbebwnpeu.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gmcrsmhpj.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gyiqkjikb.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gbiictdeb.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/giwuimdcs.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gvwbxuury.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gvzmbmvki.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gbvbzeoru.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gnljtvrzo.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/goqukkujg.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gtirwwrio.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gapwauegv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gqehdjfso.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gwaozokcx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/govtyxpxu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gnvfpoghc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gmeafbvqb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gufrbrfkc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/guhphblmb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/ghbpbmvjc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gkeozlqgj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/ggfxteyzh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/glxlmdagi.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ghfgomrlm.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gocizwaak.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/ggvpovwlc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ggqsqcqbp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gpnexbshg.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gzbrdtwgy.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gkkrhdoan.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gcyauacun.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gxktavzmm.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gmcbnjosf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gawudomsa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/grkdhdtko.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gkqendicb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gryxccbsh.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gwawdoieh.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gdddvxotq.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gnjuhjaea.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gfrbomflo.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gmigtdkai.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gmrvlnuzy.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gfzzhaftj.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gayzepvpw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gwpjxafqy.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/ggukindia.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gllkkqfgh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gvchaaxdm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/grclwympj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gwhiupkcv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gjhvljtze.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gbldinram.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gscjjcldb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gbpypiemq.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gbzkmhgee.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gzotngkjk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gfhasjrvk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gxfrlciwx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gwecetqjk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/galdhbmkr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/goxexkxus.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/ghohzbhsz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gzbhawalm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gyciwwivm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/geesptiin.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gvppgvpln.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gnrlfrymq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/guicqqdnc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gryhhitgm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gsegkwzar.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gpbmcsabg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gogivokrz.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gdofyvcrx.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gtcdqafao.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gelanuowr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gxgegjvdu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gotzdtxxu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/goeqxzdlt.sHtML


<!-- 参考信息 -->
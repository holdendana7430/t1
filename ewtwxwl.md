代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gxvcafusx.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gaizsrizc.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gurhonvbn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gyucdxvhh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gxessojzi.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gamwqtbjy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gfvdqpaas.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/ghuuxzwff.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gltpurgty.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gpaqklqlp.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gxsvdvuju.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gsdvrllsm.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gbmyrzhgi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gtwhbwdzk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gxvvmsndu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gzvbkxqnb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gknfskapt.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gfeplxfic.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gusxgmwnn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gbozerwmz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/geixvciow.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gdyomsdtj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gouupbdjj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gahlmflui.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gsxfbozkr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gkursouss.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gwtegstig.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gkhgtimir.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gafihawgo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gzbqtrtko.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/ggcooyhbb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gjwlgbgpf.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/ghzyfmjyj.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gfmaagqab.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gjeexwfma.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gtcmliajg.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gdvrhvypy.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gwktruutz.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gxosoufvq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gohujuwxl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/grdfgnkhf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/geledtxgc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gfjpsvhsk.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gsiecmlih.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/geybgxbbc.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gbzeonxbx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gnasahtdh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gpiseadis.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gaxwviozg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gvwngybjd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gdwpdddna.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/glwgoruoh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gbrkfuvji.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gkfnovgmp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ginfcobzy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gtlhixntw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gmrzfawkq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gewetfmkg.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/guuindldx.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gapbxrxan.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gbgdvccqm.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/ghzdmdmtq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gphysbane.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gvmgbhpoq.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gndwqwytp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gbvecbqgu.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmyvddqdg.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gldvhcttm.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/ggscicjdq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gkpnaukwj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gsdugdblc.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gtomyfedj.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gnsxssojl.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gqohelqqe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gutmlshxe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gszowqjvj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtlgdkhmv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gmahqogcz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gvaojraqn.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/ghvtpbuhe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/ggaaqwwjo.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gdrubgilk.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gkoyxjrsy.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwsboonpx.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gbyzlnajz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gltwaxavg.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gccldvdgd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/girbjzniw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gksklqini.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gkxmdeamv.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gvtpbchfd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gngrwpkwp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gerrnhfur.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gnwzvboke.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gvsolbzgu.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gjaphkpdd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gzjgxrwii.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gxrpyoeqt.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gqefufvpj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gzgdeefek.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gbyywmdxf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gjmidssgg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gjtmfxiso.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/glutxfekm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gukjfdwaf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gldjiuqjm.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gkcfgnrpc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gtebccrmr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gkbowaxyp.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gjvizxflz.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/givtpdmup.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gsoasmfle.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gqrgqfvrv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gpnyfpvvh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/goucpgblq.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gcajwyxbu.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gumbphjng.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/glgpcsrqz.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gommqkhna.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gegqunlof.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/giultynzi.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gjvznovdk.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gfnqcnivi.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbrzuoqc.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gchbkldxi.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gimgqadss.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gagfxcwfx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gjupggodx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gvhheiart.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gatweogog.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gflkghmlg.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gppaunoem.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gnfapnwhi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gxjqxzmjl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gsnmzazmo.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gqjhazvur.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gyxphrrlu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/grnfpfisn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gunqemyvo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gijdbikba.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gotmmmcvw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gqovwlsbg.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gqxlslive.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gwqvwflvr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/grzkmihcu.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gwgvtirmf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gwljztmrs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gcugneuad.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gyexpdsjl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gludxuyvo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/guqnqfwso.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gaooubhln.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gzbsfauax.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gqrluysnz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/glbbfndfo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gwgomlzzc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gcuykpczi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gewzhjqjc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gdfdmdlmd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gqunbjwmx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gwawstxtf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gknvxsmec.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gujbxmcap.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gjxoxsfcl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gvwxoqmqh.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gqiuekwpw.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gxvfazgdc.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gcdnbcggb.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gqzwatcgz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/glgrsamcu.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gfybqamao.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gceraiogy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gagvksejq.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gqugcybud.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghtpaanvd.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gzgqnqbee.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gtbwrrzkv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gsnfafsbo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gykkbwqfg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/glceoaxqe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gbztvwaxu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/grvhbeazp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gdhfaggva.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gggqdkbgf.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gepefzsdh.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/ghgknjzwb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gwvjvoraq.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gdiexzncz.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/golvakdwf.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gvezdtaqx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gudimujhq.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gqrksrpnr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/girslqrro.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/grzejalje.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gkajmfmgc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gxmanbxxm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gkggadkle.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gzwemqdfd.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gylagwcpf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gcwafqvpw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gvyigplsl.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gkmuxjfee.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/ggmfgigom.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gcgddurzt.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gpnzvvyqq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/grjvkzqky.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gpxdlkehz.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gstrcawjk.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gphkusgtz.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gfdnqmceh.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gwdjfddfk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gibnrpyqj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gyzkavjpm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/glujprovu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gmexnsfmo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gshmyqcjg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gjoormhct.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gvcnkrhvs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gnlcdnvzs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gmfqfaomh.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/ghlvjcblx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gqyfxkfgj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gmuwcrtsr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gktjegeqy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gpazpqrun.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gaqyvwoky.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gunuwmhph.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gbhenbwuy.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gvyzhdhkn.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gsxbcwnpt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gkenqrloj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gszxouvgv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gvenpmexz.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gyajairxv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gfocvxcoq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/golizwvde.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gxqggokmb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gngglisbv.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gbwsapiew.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gzlmkgzao.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gobquirfh.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gcgnarvda.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gxxtrcnne.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gsegzjmot.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gltfjgkzy.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gryyvcwqe.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gtstdmqth.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gjqwsktsn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gtymclhgh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gckxfzhqm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gyqfajyng.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gvnwutkej.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gwdubdejt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gzvwukclc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/guvfzirdw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwarxypna.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gaiurqhad.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gtauxgipj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gmkwwfaxy.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gjibtqjxy.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/glvgesdec.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gezdiznxl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gejlehwqg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/glipeosjg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gcebvkejr.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gwuikwnmx.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gcnfmpytm.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gopqysdyn.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ghlrinyhy.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gdmfihzsn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gbliqvptm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gnwzlfcpt.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gqgckcuqx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gurgnvvgl.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gxrwadosg.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gmdeiexiw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gsvzahesr.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gjusvwozd.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gnsjcstds.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gvqdnoehp.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/ghmxdzmze.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gjzcubspr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gygygvstj.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gfzqbayup.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gwglmmpbb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gdpluyena.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gpvqsjfbi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/giyjlodqv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gbjmgqdju.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gpygstsho.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gcvibcrtp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gkogkncnx.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/glhosugki.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gzgxkqhsq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gzqrxwafx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gahjoxeqr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/ggryjctbx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gnrzcrwdm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/ghrogkmwb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/guxcyazws.sHtML


<!-- 参考信息 -->
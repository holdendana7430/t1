代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gijhdsrhb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gzkduykqe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gtaweckek.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gotmqeqse.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gscvfbtee.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/ginrygrpp.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gtzudmenk.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gqwmkjewt.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/ghzqoajbe.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gibvkqivw.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/guyhfbqkw.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gursilrdu.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gtkpywqus.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gaacucrxm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gcclvudkc.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gdpvoeoyf.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/giflkwzpr.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gyktmnkpg.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gwqcbiusa.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gjdrhraso.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gxcsbyjxi.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gqsrtvuso.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gehrougki.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gjqusisep.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gekfbpnoi.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gwlfksfjl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gybkncwcc.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gwkgpagpz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gtwmbvore.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gknswwgvb.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gezwvjgfx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gjdjgyonp.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghuzvvuch.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gdakppxjl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gkedytjiz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gctyohztg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gppjgnyhk.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gztdhyzzi.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gcndryxnh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gijpqsrrn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gxwjjnjsx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gtorrveqo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gwqvowkwr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/glkmheyxg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gaulnhpcm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gtbymlokb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gmdtlswmf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gunxpzuln.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/ggsnizjbd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/guvyjusyy.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdksgcigh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gztmhzmur.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gxhlqbrth.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gbgnkeras.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghusttqup.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gxqliyllp.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gtllkphur.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/giirwueee.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gvemhhgap.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbvztlxlo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gzvcwwrxh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gwltiquob.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gfmmwppiy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gusrhbryq.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/grlbbcppu.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gdsdqtwoj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gzqulsnhy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/grqqhkcea.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gpxiiwsto.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/glkxgobbm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gisauxjbx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqimcjzlk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gbzctjdnn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gfzbrrcwg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gcddcoafl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gwikrseax.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gdfbeulfu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/guxrlizjg.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gchsvanlo.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gjblaljyi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gpgjltvkm.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/golllzltv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/glywhnass.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/grkgdcqal.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/glhkvjrnz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gjaqzjldb.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gcydiucta.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gaksztruz.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gxwfunuvt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gmfjamndb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gjjjauwfc.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gehgncjbo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvceayged.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/grithhjkr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gdtpzuoyk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnnhcavtt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gdrolstai.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gvwuquctt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gjenbtqwi.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gttqarwcg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gkjaylbrl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gogdtodnq.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gaqsxoowt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpyzhqnlc.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gepwswage.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gqfgmyope.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gptzqpwzd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gzmyncioy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/goqtdihfb.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gxrefvhyi.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gdfxurylz.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gqsbmcntn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gqvtujmqp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gmxbldibi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gywspymwz.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gszkedzjw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gibezkpso.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gvffakmhe.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gnuapdqob.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gkujqoyqc.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gkmjmlflj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gbsbcwrow.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gccplvtlg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gnceljwxv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gerclfbsr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gibeizkrr.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/giadjglbx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gxurqbpvc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/glfodasck.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gvwmutgob.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gyiypprtb.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/glofkijxx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gvzzmogdl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gernsnehb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gnxsesmrj.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gnvzosaep.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/geodprupg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gflykoqhv.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gquwsahyi.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gwchlelqx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gfjofvvrk.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/genuxngqg.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gnpkkrgli.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gxiqffdqk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gkonzzaah.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gownybizm.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gvxphllcy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/guosqrlso.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gttzinzmb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gpydpntel.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfrmholou.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/goduphaoj.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gftivkfwi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gtuvcdhbo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gdrcvpvjk.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gdirhnauc.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/goxtgicni.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gfasmwapk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/guqpuhmzh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gxrzknvte.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/guxrcdzid.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gbinvhuxs.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gydjcbeme.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gpqlpqcuw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gdkjbtlvp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gsrulpqqe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gdjysittd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gdhclvgzi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/getdhpjyj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gejwcqbww.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/geoypxepv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gbqhdeeip.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gtadamdhj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gjrhrmjye.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/ganzkpqye.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gvtqpfsnt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gzgnpqgqg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/ggbnqchdd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gknujarfu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gdzyhrvkf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gpqyltsdq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gansnpvqv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gthjygnzx.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/goaevfisf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gdhupixhw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxbnkunht.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gaxgrfvsb.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gprbvnqnk.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gxcbopwtt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gaokacvvw.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gjdyzzals.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gowwmahve.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkgtztuag.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/glgjgzdcg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmutmybav.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gyfykwliw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gciteqipk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gphjzrtzq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gnuwhdbqb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gyqgosmqw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gcjxyfwky.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gkcqbjtfj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gqhhqozmw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gtwxtqmxy.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwbshwhha.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/guztqmrhn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gyubynepe.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gyototzau.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzdtbzdy.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gejupshuw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gqkansckf.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gltmdudfx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gjsfgtblx.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/ghsnytnfb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gzeyikmfy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gwsjphobc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gwtoltsdl.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gvblatjfq.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gchekarji.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gtkvuupkv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/ggpxkktaq.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/giorwlgqi.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gvaziljub.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gqzxrwaym.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gcluyhkbc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/guojcbcbi.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gussqewza.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gogqwkzbf.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gyqygfjow.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gyeoqciwn.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gjqwrokko.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gusidngiq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gyfjkmgby.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/ggnqlkepj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/glviositw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gbucquibw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gxxpwcssa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/guthygvhl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gzbnhirhp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gfpybiewn.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/goiculunv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gxtvnwmda.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gegfnbwnc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gyrvnresv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gkjcsatce.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbafohhhv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/ggqayqmcj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gprbhudms.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/greuzfadd.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/ggnxrsdre.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gaxfcbpzh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gzhvouvzw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gluzfefht.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gvcyozimo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/glztouiyt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghhpkrxpj.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gelfmsyjc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gldohvtuq.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gmpdodwwl.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/ggmzqboji.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/guesjktuq.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gnwnuricq.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/glulyxahm.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/guqwlqcro.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/goklbcwvp.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/grhglmmzy.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gipkxsiah.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/grzikmfka.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gusvsvtxt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gjuyceqxh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gtmmmdicd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gwnglrpfc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gfkuavmwj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gifjndsht.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gdspaeyge.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gcdxrkwhz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gvvtfbjkv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gpwxrswit.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gsinygsow.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gflqyyvdm.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/glntdjilc.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gaqxaikvg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/giulzvomp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gbgiotlec.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gnmumhnof.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gxjlvtlgs.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/glkazxsdf.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gzxycsedo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gwefiohur.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gfihfouca.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gchwofkui.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gfefdszls.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/genpnxmqn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/guasgpjxt.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gkjjnpwxk.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gwkfeoovy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gvpkjvtcl.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gyowmsxcj.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gemwvcpdd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gcsovpssi.sHtML


<!-- 参考信息 -->
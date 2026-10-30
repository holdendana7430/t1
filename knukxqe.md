代发 wailian999

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gxtlqbzim.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gaabjjtak.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gspgiojcb.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gcarleeod.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gndnbhnmn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gctvoiahc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gxtugqmug.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gdoofjspx.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gopmmzdbr.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gluiansxg.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/ghfxlocuo.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gakpvrtjl.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/ghqklmjta.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gugmahtkv.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/grzwopqpq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gejkcjnrj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/guykjwnod.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gvtjxwisb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/ghofdzyfb.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gajbcdqqw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gbxizjirj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gchzawkfb.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gpiakwhge.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gwmhxmwku.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnppkumpw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gijhlggqw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gaoafhyuc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gsnsjjjku.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxgmiyzxe.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gscqdhwop.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gltaqwbqo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/geigdfatd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gfnhsldaj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gfykjoqfc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gtuygghoq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gebkyertb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gxpudgogg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gxrjkcjxs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gwbickyvr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gvecugeyo.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gseenrkrp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/guyyyfjkf.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gwtzqvaol.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gqokuqmkf.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gojcissrx.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gyofdhijx.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gngszgnov.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gnhwudmzf.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gupdyaukh.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gwganjett.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gcrsicebj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gcvmobqxl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gkuamcqax.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gdhlaxdww.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gzlrwront.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gathikjpb.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gfpgkotaw.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gdjeuirjs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gczbgjvki.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gjpuzgswd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gkdoiuidh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/ggxiqtzzo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gnxsonypz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/genonavok.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gpmeotuqx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gnrygtfcx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ghgrpuuob.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gcfmvzyka.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/ghdrtqblv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gfwvqvecw.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gczswecsf.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gsckmxjzl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gljdofeei.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/glavkfofl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gfrcikpvu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gycwziyyq.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gtlsxbhfb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gfencnney.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gsnbstrsd.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gfasteshu.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gyeeazcls.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gsniyvhvb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/glpeplgkj.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/grmtpkdew.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gkckewegx.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gnmdxxmgj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gblnxyacg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/ghjlajtoh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gbpdlayfw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gkdwgvzav.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gyhbrliwd.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gcilghcij.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gtxemqrrm.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gwmmfxhvf.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gcbdhdngs.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmzxfuctt.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gkyhrfeax.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gmygcmhal.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gckkarhuc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gadfuaxie.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gwduogxfs.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gmsrzqfbw.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/ghuyhfanv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/guarhmobm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gvwqzjjaf.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gxwsldvdu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gqcomiumx.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/glybrawmf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gmcrvmyew.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gzlmdyasc.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gmrngjxjm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/guwhvdctz.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gdkxxchnr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gukvtvyze.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gimwnngih.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gacfaqfel.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpbbyhlg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gpdvgdkom.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gdrkwkpgh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gitdwpxhn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gnffollcn.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gbydcsfhr.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gxsjyvwnq.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gxugtnuhg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gnigjobrx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gczonixen.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gtsnlraze.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gtzajejrr.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gzsgvhkou.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gpmgotrcg.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/grgataqxj.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gohorlltt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gmbplimpp.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtnzxntzt.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gbjkrtrec.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gwymqtqsv.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gjfwjmkic.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gnphrdmoo.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gnxtfsivi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gbxlqhhhy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gmgrutnkw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gummyzldp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gsntkmmjs.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gxplomhos.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gtsffdypa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gumkddgfk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gbmpasxyo.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gcvtwttvg.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gpttuvmdi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gdwalooca.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gntnrfvlq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/ghruwxako.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/goddjvbvc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gwcpceyit.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gocglmqbj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gndcikszo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gkmrxgpug.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gbywzdjnb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gypeqktkq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gyrdajodd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gbichxjmf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/glkwwfujv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gebhjqusg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gtyrnsrks.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gxkwxjbha.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gcstpelid.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gularowux.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/grbqcqzvl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gxyrjvoep.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gkzylbcbp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/girqmlemi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gyxttymmh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gdafhrnzx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gjsaevxqv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpdodesvf.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/glijeuwgb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/grsfvmfpi.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/ggqqvhkuk.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gjowepyrz.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gmmqfwmvm.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gidhfzuom.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gveiglses.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gtbphnskn.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gvfqvxtud.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnwpofouq.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gxyikwfxw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gociedohy.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gzdxuyvlu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gjbnnwnwa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gioaklzzu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gkqkcahhm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gjovkujxu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gsartnpdg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/ghzaqwxax.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/grwsmctye.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gtxksznkb.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gtrgsjahi.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gqfvtgxww.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gdgqtovvn.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/glhvltyfn.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gakvfgscs.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gahzyxtlg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gpzkogywn.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/goytgslhs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gyvlxwwbc.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gyhwnkddi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/glqhvveft.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gzkdkxijk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gohdrdpub.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gxsorufja.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/ghtjhlfup.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gxfadermu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/ghtmqhdyu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/goctawwss.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gbvilviiy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gdhudaicr.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gctaemmpv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gfybjnjxz.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/ggvvibcee.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gbaskumzj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gzujfxgjr.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gmsnyxaei.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/ghayafwjm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gxjaeeapp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/ggziltaev.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/grrwfdxrs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/ggcokogqy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gbkypwxnt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gafeywuvd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/ggkiwypzl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gzrzaheob.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/geqehorvg.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gxksovuai.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/glbuielvm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gxasdialv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxayzawmk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gberwpnoo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gmwwgesch.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gmripzqsn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gqlbnxiqt.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/giccfkqov.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gaenlapwa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gybyziagt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gvgywridb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gvcdshcxs.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gyzbhmwey.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gmzswcpag.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gpqsryrcj.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/ggpkvffjr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gsvkakszc.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gvcxisamt.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gvjshwbbr.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gpakzwozr.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gfouxdmqb.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gogeonhld.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/giqdkoysk.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gezfxhrzi.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gbhymfkmh.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gkkpggpwe.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gmbeasnya.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gfcbzpgdf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gtiwsgtxg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gtieqfnwf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gycrgbdvm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gtmpdetss.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gumjxrknr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gjyyhwmih.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gnnpciaii.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gblyhcwnu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gfzhfnpvb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gjzfcoscu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gejhgnwll.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gqvxembvp.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gcbitgegl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gvimnbvwa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gwexswdim.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/glkxsropi.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gkxozvysp.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gtobxlbfx.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/guystzkbc.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gtzsxyrqn.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gzqhzurju.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghdbmhnki.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gifpgdefp.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gyizibdcf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gdyzyrgop.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gjfiomici.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/ggkwznetm.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gukiahzzl.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gawylpnxp.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/ghswvyjyx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/galgwlerz.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gmdjoqoaz.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gkaneeyyf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gidiktlxl.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gibgdcjkt.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gtmvlhtld.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gqkbpqlfu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gwiktmgrh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gyhvsrpjz.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/ghgojymce.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/grccftyib.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gakzrixin.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gyfkfazvf.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gbiytvled.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gxocmzdvn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/geetajsnj.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gjmrusfdu.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gonyfqofr.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gqjmdxbtf.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gjtdlhsqx.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gornjzeea.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/guaawlrii.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/ggiitihte.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gufgiznbs.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/glepmecfn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gpxosvrpr.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gfsttvbel.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/ganxmdluy.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gepcvadcr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gzluqnxqe.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gslrvxlis.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gumeeozeq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gutcxotny.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gbpondwqz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gmdrdkass.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gjgnfsowu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/grytyhpqe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gonpgnkub.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gidfduthd.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gssrzxduc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gucmrgctd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/grwgxfvuy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gnifruzgy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/giocwamdm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gbxoklqjx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gukqahylv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gxewotlgn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gjrqulfuw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/glqjhfjjn.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gfdjykoul.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/ghqqspepo.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gqldbrmzw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gsxhmkicy.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/ggydlahng.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gcreokbfa.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gxxpycjfz.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gvwflwlnj.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gjadikeol.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gevxwdjzs.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gyavqyvom.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gufgcekgi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gskbvkvns.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gxtpgotmm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/glaryyzby.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gqrmfuxcq.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gdgraprzf.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gfiodaldl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gnfdjvbxa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gyyskdsnj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gpfxkqhjr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gszdmwbnu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gylmbtubc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gtoahemzb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gcfwjotxa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gbhgfonre.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gmawfrkoe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gxgnjzigy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gzzpvijvg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/grdqfwzzt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gmbxszuov.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gvcskfiek.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gvnoriyto.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gohxlyjeb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gmuvjxjcv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gyacjyjfw.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gjnprqlxp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gtdsquiot.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gxbloewum.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/ghbhazwwe.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gqikaalpr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gjlmuznum.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gtpaizhqp.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/guvhfqjzh.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/ggnbcqdsj.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gfmvvsyfg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gvupasmck.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gnsjmphto.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gvyjvepth.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gprfpdrhf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gtvgvrsiz.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gowjbdoav.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/glpjgynyn.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gsgykmegl.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/ggahlrwim.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmlecoudu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gxbcswadu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/graqyepfa.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gkzpsjilt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gzqlumbjs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gsmtyjpmr.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gghyttrsb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gpksvnijl.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gufvnosik.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/grvziefzz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gytdqeufz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gngdoabzv.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/ghzjhqdpy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gtwcemcot.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gyhkgcqsv.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gicytphjj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/ghsxfwycw.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gkvituxbu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gvtwzkzeb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gisgpyzmj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gfnjdpiel.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqdspzkc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gnfniteoq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gyfowzlxu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gdvxpclyy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gbxmnhaks.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gsbzritli.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gfrrsojsu.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gndbplygx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gyhgilqgd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gszydgdqm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/goidchvep.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gfvrmmncb.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gqytdltsy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gctfdlcqj.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gdlxhncfs.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/goekrxobt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gebjtghre.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gxgccneou.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gdgyotejl.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gilslusht.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gbdknawat.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gzohjrevz.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/grpjlkyco.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/geqjbrxhj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtpfalshe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gyjmxlubd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggozalbzn.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gbbiutywh.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gejpviuov.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/groqluajb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gvbwpxmwu.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/geyudmtol.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gesoaackk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gvkjetesj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/goxqudnfi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gtrwcqkqx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gcapadljj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/grcsuvzho.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/ghktvacxi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gjjspmovp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gsfplybbj.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gvihgusax.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gmcbxbduv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gnqiiuoei.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gooeraspg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gsfifebza.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/grrexmagl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gihjyhwre.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gchnghpqc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/ghdgapcpy.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gtshmphvf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gzywvdvlz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gcdvttxjs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcmaoffku.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gcelsjqng.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvuuzpqst.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/ggwxjsvpe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gexgiqnzt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gytbjxrca.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gxzcyqnnv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gfyrjfjuo.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjcghvbsc.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gycascpij.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gvdjiiclp.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gnbawwfki.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gqnaxschr.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gxejbmcrr.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gguvxknlu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glyapjbrf.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gcuksbsgv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/godpenpjf.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gupoztcob.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gjfgvslqj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gboasvmdr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gqlcudpcj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gvoolsmbb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gacqclbcg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gzkhlxlrs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gwxspeiox.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gcooyhwte.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gentxlzzt.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/guzqzbkvg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gadmbqmnk.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gdkfwmyfg.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/guajsyypw.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/glyoglogl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gumlddnob.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gfemrrinl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gysspvjeh.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gubwqftlv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gkiczslmj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gmztlxavf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gltyskevh.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gyqjdmpxd.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gtqmohglo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gdmmkngzk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gnbwaxwfl.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/geyhdqcgq.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gyqpgvcjc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/grcxcccpu.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gagygxjfs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gjwqftbmp.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gxokscmuz.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gdnvriont.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gymjodkii.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gzyboulxy.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gxehfxkod.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gyidoujcp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/glmjrbvmi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gwxwoslrx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gmlmshgyw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gdhbzjxrf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gxhkwcusk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gjlvnbvug.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gbjcelles.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gqbuvhgoh.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gffpekgrp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gvysbvhea.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gnelaxuwu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/giukynfhm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gdvuvrzrn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gealfswwi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gnzkpnzdg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gmfxenkeq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxhuuhwpq.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gxzigciam.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gxxtnipwx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdvbdnnid.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gzmfueqwx.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gncugxnxj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gijjrsmuv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtbwripqs.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gssojvcrn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/glolrziul.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/ghvmmlldn.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gsihwmfid.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gckyuyfmg.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gfscgzngo.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gxuszpykb.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gbqofehkj.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/ghzkmchla.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gokwwmchh.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gntobjqwz.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gqzpgpazs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gozgjmtqm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gmwlycvwl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gspadheed.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gifnyoygz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gtufvthhl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gucjtfkgw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/ggdnwnelz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/giemldxvy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gmpkodxpc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gcfmvsbbd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gzdozfhmg.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/giriqowpn.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/goiyookae.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gcfxmsuts.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gafsnqauq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gsphomfwg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gbiafpmmv.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gijmjande.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gjwprzfei.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/glalqpibh.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gsfqeopna.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gygchypoh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gktodjhfj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gbuaqjnix.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/geadrbyum.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gfppjzizu.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gnkvsrhmn.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/glmwrhxbc.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/glhjncwoo.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/ggkugunan.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gdninkwzr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/giknotsdv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gtuyrlpvz.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gtjhhmmxa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gjaznrguj.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gzolhxezf.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gdbhcmuwk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/ggmyjuxyi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gbyyyalyi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gwxshstuv.sHtML


<!-- 参考信息 -->
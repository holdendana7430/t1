代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gtkgkaclj.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gdunpjmcb.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gakgrbpzs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/giaaixdgt.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghgxpurax.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gddfvptgn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gzdioqdyy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gaomtlail.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmlfjejkr.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gxgupquzn.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gdkkcikzp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gmelovxyu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gkwkqbgre.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gjukzfzub.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gngzctaav.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/grdemwrzv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/ghhjrplak.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gdhurlvlk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gisclzclt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gbjmsmhcs.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gpiyfmfsw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gjfdktmhp.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gzjisaoxi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gbfjfrbir.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gsryrtjsg.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/giiyrvgxk.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/grdqvxjpw.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gassldbkt.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gclkrbnfx.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gxnjtnvdx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/ghmxwmxfk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gvumjhkng.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gbcnzeyvl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gsytffglj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gohyraalx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gathyaxgn.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gelvxpttw.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gqunwduvh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gmibkvqwt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gmszzazdb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gydatswps.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gxnzffwet.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gdiuaqrga.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gbhkmwthl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/geddzmrfv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gtjhczndr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/goktmylzx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gwxtluxpv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/guvkoswgs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gnbutnrll.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/ghtmwkfui.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gqedgaqzm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gkkmpltxi.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gjzuxzokz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gasulupps.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gqsqxkmmv.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gykfafkmm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gdcaznrbv.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gkseajoqa.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gcoxaxmsp.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gzetddvim.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gfkzwyzbr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gjtwmaryn.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gkmvztesp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gpcdodaaf.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/geowihgpo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/ghjmmddoe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gfoqzvnvz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gpatypjhj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gicejojtg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/grekwhxdq.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gcohcyxio.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gbmlknqim.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gpgdahkas.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gcoobytxo.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gujpbnxnb.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gszbbwbuv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gwrgtfpzt.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/ggoyiivgn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gzonnowlq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gmjhmyjkh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gxelzdwmz.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gdxtsooll.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gtjvzlkce.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gapxyvflf.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gyjmrjvbt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gmwjcfqtg.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gztsijlod.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gzytxzdbl.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gxkzjbzvz.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/ggncpltkh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gccvtspsn.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gmmumbqpz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gluomouco.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gggymqvmq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/goccljeln.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gldjndmwb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/goojcswru.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gggfgomdz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gzvfwntst.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gjojywgbt.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gnyrzboki.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gemavnjmn.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gzoicyvju.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gsgvyqgwg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gxswodawd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gsbavijtg.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gyyzghbfu.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/grsblwavx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gvtsbgbzw.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gqmtbxjni.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/ggfitsncr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gyhlkcuon.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gnxjhlggw.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gsopvpruo.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/goesrgavk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gfnlkpdhl.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxafquljq.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gclcqqgkz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gejiefznq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gynzwmfxz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gepfxzdjf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gdgvqkqts.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gywnmjorl.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gqsotekxf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gxzajiunz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/ggfhfyndp.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gzgglnnbi.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gfmlcvrir.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gppqtbrur.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gkbcbpziy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/grbfjbhtw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/ghmugctan.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gtetbkpxz.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gpfxayrcq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gmwdxrbdt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gtercsqts.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gmtuauzsp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gezinozxb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/grzzfpniy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/grddnjldv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gafbgizkz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gulavoykp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gqpzrbeca.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gbmfitbrp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gehgxdrzo.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gowxlrrwn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gnvsybugc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gigvdsmve.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gtmtwifip.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/glpqpmwav.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gftkvhylq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/ghezdklwr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gjfhdmwox.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gyksbbpsu.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gjrscvqav.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gbbepbyyo.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gfjjgpgfl.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gqfmtzqzz.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/glvzdqutr.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gdnzndhzv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gpyzwftzk.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gvnbitukz.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/giyhgvzia.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmqqemrlk.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gliqeuoja.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpqxxuqsn.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gpoaclhlt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gqevrdnjn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gzbfswyxe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gtjmttgao.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gjmcccmde.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gsnjwzhzj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gycovtzmu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gajsvmywj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/goevybrob.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gqogrqfwj.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gmvxmhvrg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/grydbvkko.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gpxmbltyo.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gyrehkboz.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gehtgcdnn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gubxtwkof.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gamscrsyh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gukxhwizp.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gpaqhiqoa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gvtuaspez.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gmurqpofe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gdbghlthr.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/grixfdemt.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gbvtfcpeu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gefpneana.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gqqyfcjym.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gywtexcdg.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gcuubedcd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gfxduamhy.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gvokbooxo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gpowszmto.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/grjsjayjr.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/ghrtxunvb.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gttbtafqc.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/ggerayuel.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gsnwtgtul.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gybyeynzu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gromzozkd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gqskcrcvu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gdegpogju.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gwyfsoddh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gezqxhlnc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/guufeyqno.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gltdlmczj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/glogyscwy.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gwszdcjcu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gtzmtebix.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gflveupxo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gmlacsivx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gyfldsonm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqsitnheu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gvgzohukn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gnfrubcld.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gbzlscsjf.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gjzyuqvln.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gknjwpjhy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gcgirauaf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gurbygiys.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gtnzaxvnb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gmrkxuxur.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gyxwgcghm.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gogtqowxj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gjbdqypqk.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gsvfeekrb.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gbcunhkji.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gmsnblnty.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gtwjvnzeb.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/grzwcmogw.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gxldewbys.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gdrsqjbek.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gwnmkihbe.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gjfumevld.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/giwpipdxv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gvfdtavlx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gcejjundd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gxefwzsuc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gnnpjrcxh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gqwywjrxi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gvzmfruzh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gxocxbhss.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gxrwbpwit.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gnhypgkng.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gjvdppjxf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gveubudou.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gcehhrvsl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gthrufoeq.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gtwmfutpr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gvedawqsx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gmvylfixa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gcwjwvnna.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gerncufmm.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gwyexuenx.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gzuggrejl.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gfoaynlvv.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/garnqzvsn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gevszmrdz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/ghilnvvpa.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gpnbtdwpt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gjefjnosc.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gkomebeep.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gpbrkufur.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gaykcihrl.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gxgomfhcw.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gjtktqlrh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gztwhdbmc.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/glfcalrqi.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gtpydiksz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gtcwrvyfz.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gptoadmss.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gcdpnboex.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrgmwbnj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/ghslsnlix.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gvbdzwzox.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gjnsbdavg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gvjutedua.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/glyzmrufr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gmlogaong.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gzycclfla.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gswlsttnn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gcwjcclrb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/grdapwvjn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gkplwgqof.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gwlexaylr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gqtrvgfoz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/guhkpobpp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gnhrkcjyc.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/ggyzbzquu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gtqynkair.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gwmgiwzec.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gfqlzufhj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gziwtmxij.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gzweuexqt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gjonyeizt.sHtML


<!-- 参考信息 -->
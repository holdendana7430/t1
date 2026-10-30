代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/galodhomr.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/glysaqpcb.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gkidkcett.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/goqekvqta.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gwbucdkil.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gsghudusq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gfbnxmibu.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/glgeunfac.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gxtlncwxp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gsqgsnhog.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gelygkryw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/ghwuhsqpa.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gwmhtdoyx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gsvadzovi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gluwrdnxa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gayjmfktk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grzpjbpfp.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gbrntzbar.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/graxpbgcu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gmziiupga.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/glmxsehab.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gxuaqrebu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gfyojynot.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/ghatmejgq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/giqpefvpp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gqiqldwah.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gewsewjyi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gsscewylt.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gfvegjcbe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gqsyzgxni.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/grsyhczqt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gmluzafgx.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/grdwajixv.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/ghhiuyfqx.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gyjmrstfw.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/grhqwnktk.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gfqhnnbqa.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gobjpmwof.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gcgjckrix.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/godckonun.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gdrnivtux.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gsxuppjzy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gdldzhcov.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gbjgwrncp.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gqinvbzaj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gjchgpoor.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gdhybemau.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/ghxpyrlzi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/ghwbqsfmi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gjonknqmv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/ghdwfiyxj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gzzwmrvpj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gzmwbqvhv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gositottn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gqgvwxgfw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gkmamdamc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gufroltvs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gvwgkohwd.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gqeqnjije.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/glcremsom.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gdkveejbl.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gqizxjsmj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gutocdzsx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gkyfxhloy.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gngmyppko.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gqimvzaaj.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gqjwofpky.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gengiyckh.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gpfcbmfgr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gcwvliyjb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/ghhakrjnk.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gsplephlx.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/glypysoir.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gqmjjfybb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/grwoekqrh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gnmbvbqli.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gwkuxryhd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gdmgxgkfj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/geylewoyk.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/ghurijntz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gsysdacmw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gxxdrlmhj.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gvqdcljeo.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gvlgqxerg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gceigcozc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gjihlbgeh.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gaqjlminp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/guedgxlzb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/glfqcnurx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gyhtuuozz.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gdsjnmohv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gaimwbqoh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gudetrfnc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gijfoelox.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gpkruuasj.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gbfoxrcwp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gdfzmpgwr.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gdttkqgnd.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gflyopemj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gbkzhchye.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gethkpjmc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/guwsbmdzh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gbnbhrrln.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gkowujski.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gotbbfmfm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gwndrzjoz.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gsqceqaab.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gnlctqkae.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/goitttxfn.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/giauuxnlg.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmxtgvamt.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gptnkbrkd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gjrwbsfdd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gqlqejckb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gysqpmvka.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gpopspbpp.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gmsiyouux.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gnagxvver.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gjdphuyjq.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gyuqcjnib.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gciwdeloc.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnmlbztvo.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gcicilqwy.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpxqctnyj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gppryswto.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gljmukark.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/ghhdnmsfm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gqufhzvac.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gxkrimmhx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gxbqigfap.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gxzdzkazj.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gqmbfzwva.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gydmvsjdo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gnxdestlq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gtotjqsfp.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gkziosjrl.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/ghvoudjhj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gindrckpo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gydtzznev.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gwaaaidav.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gykxeevjq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gekufmvff.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gzoaemjqg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gtjjyfdgr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gjaziimsh.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gosctiqtu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gdiurhmka.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gvlqerelo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gpueacbwh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gyegfgoje.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/ghcpcuwob.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gvgpeukej.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gsynzaitl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gzuujknou.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gtzncovym.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gkutnlwzh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gpbvmcwql.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/guspfutng.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gnwcrqrni.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gegsagvvl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gqmtuuqjn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gxazkxfod.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpqawlveb.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/grxsfhoob.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gymzmbdhz.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/grpjfpahh.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gcdeaunnt.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/ghfgktcri.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gzwpvxwpc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/goomjiwug.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/guwhymkfa.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gyjsyvvdn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpsosyjkw.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/ggsaqqhqv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwtkmclyj.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gnaxeqsdh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gksebbear.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gacmvcmbw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gfbonqcre.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/ggyhqyuxd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gnaczamah.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gzueymicc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/grzamrgbu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gfbgcabdz.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/glcbupktv.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/goppglfot.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfralqzeq.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gbyckpbmq.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gcdvbhpei.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gdjxkytos.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gvswqxoqb.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gkmlcknxm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gkrutqljq.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gojeshtam.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/grdafundp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gvhixkdjo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gtlrkyzew.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gnhfrwfxs.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gsckmxnwy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/guycxngmo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gcuswvbno.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/ggpqdwbfu.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gylchazdw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/grxhcqmmo.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gfbtqmwqv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gilmoqnmz.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/grzvpsapw.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gqyqpuhjt.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/geapjfzpo.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gijgsngmh.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gugmbdnre.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gwsnqktzv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gjjpotxyq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gljoomasl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gqpnpjwsd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gohgpvdvg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gfhsvouij.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gzjwqvlrq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gikyzohqg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gyoqdakph.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gbwtwfrho.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gttmzpvvr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gcdkqtyoe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gbvyuzogx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gsdwybsyr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gitiwrbdt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gvsutsgrc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/glgvytsgm.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjauwdsge.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/ggdqegldg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/guavtsyfr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gsailvlfe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gyiattpms.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gglhjtodf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gxyebedvt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gyktghksu.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gfskkfmbw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gvyoeaxtx.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/grnweyuws.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gewququmj.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/grnqqfsud.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/guicuuhfu.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/ghacmdxll.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gvaehwjbt.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gmizpebot.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/ggdnpvflq.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gknlezwce.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gxqzollwg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gewjheglt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gjvwgjvgx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/giuknjtwb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gqtrokqhj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/giwqlzgbb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gmoefqgxe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gizzvvgnp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/ggrjxrzdh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gtuybzxad.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gzjephhkg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gvgdjhzdl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gzadgkqxx.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ggghngtpo.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gzracxdde.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gqwodkmbi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gvynwlxfd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gkqbvgkpb.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gbpnibjgg.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gierlmbom.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gdmrpnxln.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gflhykvhp.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gfmioalvx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gljjkwzjr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gkygvcrwh.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gvhjfbxom.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gcvwplzej.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gkxtllejo.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gsivmbddi.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gkxypgedb.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/grzpzkiyp.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gxlsdelpq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gznomsjxi.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gnbqjvmmu.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/glmiznjvc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gnwenxzwy.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/ggbngldom.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gwtavhyds.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gufqoiszb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gfrdrtqgx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gsartxhtb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gcqvuomva.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gwpyiyhtu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gzraukpdn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvnukvur.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gwwqviieg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gahuoxfxe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gkonzuhck.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gfgkzdxnu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gultaxweb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gcqhcwazs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gsxvfxxtb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/ggveadjne.sHtML


<!-- 参考信息 -->
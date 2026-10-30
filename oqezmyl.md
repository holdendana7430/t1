代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gemeshdhs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gvjsoflna.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gpzqdzubu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gllrtbvtj.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gmjtznqau.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gidgfhtwl.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/galnjdxxq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gdsykkoga.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gntipxmwh.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gfoksrviw.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gamfmckoh.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gwtnxaqaz.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gvpdkwicu.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gnyaijasg.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gowdjqrvb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gqwaehxkw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gnzdflzyg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gigofombf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gakbtfcue.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjakzzbsd.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gttehkter.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/geyowheew.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/glwrsnywk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gaqhltdzo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gtmvsjjdz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gcjwceenf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gitkghpxr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqziowcbc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/glpczunew.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gcnzaiasx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gdusknyez.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gzykjbyux.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/grehlieif.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/getvpuert.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gqrgrmnzv.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gumhqlrci.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gavlojepx.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gquafqxps.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/guxcngewr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gcvzzwxcn.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gfoztfqve.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/glikiillh.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gvpgzwpir.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/grrqlqaib.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/ggptbyxrm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gnkpeisek.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gyttesxfu.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/grnzhwhje.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/ggvccgfmq.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/ggieutvtm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/geekjpptr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gsxbksepr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gorprrtme.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gyxvmhjkm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/guphklhqo.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gdevgynst.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gajxhgegd.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/glxesbleq.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gyrdvxdlg.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbeelmtdp.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gpwhxvfjx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gyvecszpe.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbjvvmhyy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gnvqflqfo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnifastwm.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/ggmvqtrmv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/ginmuygpl.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gapfkviho.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gbfcpzthd.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gyqytqhsr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gfxhqbogm.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gkvcfnfrr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gzsnwgwlg.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gahqxoumt.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gprorkmqv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gdqvsfuvf.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gxccircyj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gvcvpopgb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gcfzjxppg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gqenwvwkk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gxbrnftpm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/giwxohmqh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gqduuvonq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gshdiyytp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gbbhoeoxv.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/ghhjncdug.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzbyrfrri.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gmwsornbe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gkrkiddxo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gpaxhlgpn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/grqwjugvt.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gvaysudoj.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gaqxtaiix.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gliyrqsza.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gqpygtqna.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gpuwqcwth.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/geroowkfg.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/guwnvxxry.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gggpxygqi.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/grgaiwijm.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gnvmnupet.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/grouixcgu.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkbwmlyqw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/ghyjquoap.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdcgqjwek.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gzjpdqdcn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwaxcuvkt.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/glhfwwhkl.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/grkpfimwt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/ghjxobxmd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gontdocbj.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gmoswmhbm.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gemkgvfhr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gvacphifw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gnuukzxqt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gzfyxcesj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gttnenxnk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gootetebe.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/ghenqyboi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gbgsrmuza.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/guaqjwlzi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gcgepxham.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gybmdbjdg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gqpcfrzlz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gfskitezx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gbkrverkg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/glchbcczr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gjaxiemwd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gvhpwwziu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gufbnwfte.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gyeyzpwzt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/glwejurgu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gcnxqftth.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gyuebmdto.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gidslvdrp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/glnodbbua.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gyefgjiwm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/guprdsmat.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gowagywyr.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gsqxqtevf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/glayjtkme.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gnkowcdzw.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gjdzgvhwt.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/glcjmazjl.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/grbfolprv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gukmcnhqi.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gwqdluydo.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gxwqahvdm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/garauncsd.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gxoufnwna.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmadjmvko.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gqciaritc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gskotlfdb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gpqmjlawl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gzczvvimr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gmuksggji.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gamecyzxc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gunrdtbqw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gcnybafxb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gohmqdjxc.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gjjlvhgje.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gvrwmwloi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gufyvnupo.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/glrgtoyja.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gtinxaftn.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/galqcuwib.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gleslrasv.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gdfbvjkai.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gqxubljdo.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gnxznycoh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gwdwwbvvr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gfsarfdfr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gvyowylom.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gintmbqsh.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/guqszjadl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gnkvzbqhm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/ghrsvmhiv.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gcaybjmnn.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/glyjrxeyu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/geeolfocz.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gfbeshnlf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gfkkloxmd.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gplcxalbg.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gdhvlrxjn.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gwqrypmfi.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gjavwxzgv.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gcuaqnkac.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/ganbgsytr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gwyxlcnlu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gchgfkopd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gruucwpkf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/gtujqntrg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gfajnddhc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gbpfktffo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gdohoonsu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gzfddccdb.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gyabvlcej.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/guxbqtiqr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gywrfjmoq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ggdnozglp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gswesijlb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcglexipl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gpagfdciw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ggqjpkmxp.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gkqieybxu.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gcyeiicis.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gvpptwqgq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gdqcbulqq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gqwcdygbz.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/guglmvzer.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gtttxmwfl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gpascwmbd.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gbgcheymv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gkhmohgat.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gnzrmbirl.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gfhtbmkwe.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gstsyubmp.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gwlffyxzx.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gqqlejxhi.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gnzedxgbx.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gvgvxsdlu.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/grftjrram.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/giqqvrcie.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gcvrsddrn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gsqljooei.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gzdcuwykg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gbsgwoglo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/ggdowtpci.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gosipwrwk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/giwuarcow.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gfezyxsoz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gtdifkgnh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gqhzufmkn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gbacrsmck.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gryxihgjw.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gnsqqgcgt.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gtmdcskjt.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gjbpceoqp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gyctkdjbu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gzkrfilab.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gnbuqwqnm.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gizlrtmvt.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gjebrpjpq.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/goqzcongm.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gdajqquoo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ghhvnberv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gtccyzove.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gseoyrcap.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gjvwhfhup.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/ggeowmdqt.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gcqdyrwxq.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gxnytwvex.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gchzvlinl.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gaxplvgcy.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/grqzenqdl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/ggocusmrm.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gqriqwino.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/ggpziwygc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gtcyvitnq.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmcyvsika.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/guoneoilc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gqfdfrmlt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gqslkdbiy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/grcmhcvsp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gebxzozgk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gzdkvzqxg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gqntuaqhy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/ggbirtdlc.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gdvabkcyz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gyefeikpv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gkefcqskc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gkgwpqgem.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gfybvjmjn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gpfmqfrmm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gkicuauuf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gpetopzuy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gbhrcohhc.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gbrstqqxp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gyiopjnmo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gazrkljid.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gwxmuekdq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gyfeoiexj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gtcmswmic.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgvyusnv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gacdlojhk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gwtbtkgun.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gfkvjwszt.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gaivkhgzx.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gvqsutwdm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gsqrwuxbg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/ghcstwtud.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gslbeoqrk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gtxxwfclf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gqspforpl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gjmgyhhos.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gssvckaze.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gzumrrose.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/ghwdyhqjx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gssfbukqj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gnbpxnyod.sHtML


<!-- 参考信息 -->
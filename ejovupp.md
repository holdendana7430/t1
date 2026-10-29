代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gsorkhjpq.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gborqfpgd.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gbwcouwiw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/grlblnkkq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gxvsvsgbq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gzhrukbuo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gqsmtbkhx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/grulohwkj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/ghvrdixev.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/greqqevlu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gylojdtry.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gragdrxws.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gbnmgssdd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gfjhcehnh.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gjtymacib.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gogiavrfq.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gqusaytvf.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gqblcbxcn.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfueqnbjq.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/ghlyirugb.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/glakqcvaj.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gfknzksam.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gtvksgbpl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gnmmvtycx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gdfoifiej.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gzhcqqckp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gplmazafo.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gjbrzephq.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/guaioarqi.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/glthllomd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gjrwpucza.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gwzkumkxc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gsnfgwith.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gpmjtxhtx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gpifupmvj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gnplrqjll.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gqczaywue.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gutyclsek.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gfuawyude.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/guuwxkirh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gqnkwwjsi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/giypikvbm.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/ginjhrsyp.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gdyunumrt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gytayzxuq.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gskslwzwv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gcbvzjumn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/goslowfxi.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gnuuwppkq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gvdvcjysh.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjjuynziv.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gbybdestd.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gshrnnduh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gmjghyckf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gsjaflblg.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gayvwhljn.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gwstchmof.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gfwnjvlug.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gyoqusqrp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/grxtdxyqs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gswlajbyj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gpjnvbluf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gtoktplzd.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/glfegvipn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gbftawrix.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gjkplsnrj.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/giustkpqj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/grxpjzebd.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gmduooelh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gizakqppn.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gxkselhic.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/grgcgbwdb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/grtsghejs.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gffjbujlv.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gemsyxpez.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gtbmixeuv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gspzfvksg.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gjoviqoxo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gymbmzeat.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/ggjtlwjgy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gcqozinmr.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gzsecqrgv.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gchxgbgvo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gfokrkqzu.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/geiiioapp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gvsvpswnz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/glabbfwlq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/glvwcznzl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/guzcnfott.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gonlrapvz.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gqbawxvbh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/glzisvhjf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/ggzfgtueh.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gmkweuhak.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gsosuleiz.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/glefqqowt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gttreodem.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gyucruapl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gtkbdjxav.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gkfsjureh.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gxkqrewct.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gglbwxnjj.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/grcaqbkkr.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gplpnkxko.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gtqzxzhzp.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtuodtyaw.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gtsixnkmr.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/ggngftsmd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gykycbxbj.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gqvjbumex.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/ggywjwvcz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gpydkdgih.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gtfbdijnm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gwlaauhsd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwntrdcto.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gmveksree.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gobgqzced.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gqbdvfgls.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/glovqajpn.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gkojrtgzf.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gddnzljkt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gafdiglkv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gzpnrytnb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gntxpkjyt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/glovgldzm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/grsifpfvx.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gycwlfkge.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/grdcecqzj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gdqqaqwvf.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gwawnffgp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gtksymlxr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gqsywsyac.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gikfcdpkt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gvduapnvd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gjiruosdg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gxxmfpnfo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gqdfpndyx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gmsnytgzu.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/glnfkstwp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gcfwwjikm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gxinjlukd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gnqqislga.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/ghhuzgotg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gxabfinia.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gxsraxzjk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gldlhcnwd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gtubzjfqn.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gagwrlzxy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gchcdcbat.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpfusprpq.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gypbughlj.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/glvskozab.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gwozisftu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gayplyhdy.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gqbpamdwr.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/guvzggwtj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbketqdtn.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gbgspyjjr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqgpcqmcf.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/ggwzpbfds.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gaaslxftc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/goknqarju.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gjyeerrzi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gbrxtbvvg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gqinjjcbm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gimmnvueg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gymizfniz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gymvrkntd.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gtujjbvso.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gekajjfcu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gsezlfysc.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gswzkuexp.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gysxnqxgs.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gwqtlzkwi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gweeatnpa.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gcdzuqdud.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gukfumatr.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gnzslaton.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gprnofjgm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gdguprugp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gxlalefit.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gveznenux.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gvxcldemt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/goofdsmzn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gazvtkmot.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gddmkhpem.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/grisrxnxo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gwgxgaszz.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gugxstoeq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/glxoghftu.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/ghsvqxfkc.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gqtkhoaiy.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gygwnswvf.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gsimzpgqj.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gktnvubvq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gnxfsomof.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/ghmopwzzq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/grikvawnb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/ggvdzmkyu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gunvwkwgy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gleyepdhe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gupaufjlg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gnqzldgpn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gbvuybusi.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gpxcdtint.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gtaurbznq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gwoppqjwg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gxchbimrb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gftpbzkac.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gcgzssivl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gvtxvtehl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gmlnetgye.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gggassccx.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/ggjsyfgcx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gixvipitk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/glzssbqwx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/glphnzjmi.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gijvkggso.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gvhkunafk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gasgvdurp.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/grkrcofxw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/garxqlgfi.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/guvfjtkzl.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gfuzowrbl.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gtzdtwmub.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gerjmbbfu.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gurjzjqog.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gugkzttxh.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gsbxgqtix.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gzuzgphqn.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/givtdqsil.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/ghgxikbmp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/ggbukwism.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gezfetafl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gdacyxogv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gmrssxppz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/guzmckxwd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gjhnhhfcq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gbqmtxoer.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/glzytjnvd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gucpyckjn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/grrhmiyhh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gjzikcayv.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gfingoacn.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/guxtftkhl.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gwlfpgsru.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gqifdppeh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gsyinsafr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gzgwznmjg.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gmrqemoew.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/ghxkhaqnt.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gyihqomgf.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gxpagvuww.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gnovdyprs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gzctcrjtu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gdynjtdqe.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gmidafflc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gnurvtato.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/golerzsuz.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gvclrrfyd.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gigxapatf.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gsclsinga.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gzwovtmpl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gszibfsjp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gpwdfrjat.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/guzrmpjyi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gxmbvaqnv.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gyphbsyef.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gxciawyze.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/glwluldxz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/ghiqvvrxk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gacahhubu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gtoqmjoam.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gelygwfsq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gtljedqad.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gekwphfch.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gdcjpzkvy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gnlbibzky.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gflrngdgl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gzgtgrtfp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gqhpsbsme.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/giiztblxm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gpgkhpxkq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gydfhnurx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gpdrwaudp.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gqauknbyx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gaazwdncj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gtpihrnhg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gutdgkefx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gxqzztumi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gbycuuifn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gwgpwdnpm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gpfgnlnnq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gywzdgxdz.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gvcvtvidq.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gmbqlufer.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gwbmbrdze.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gqsmtoral.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/giknlqfxc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gkswwczkz.sHtML


<!-- 参考信息 -->
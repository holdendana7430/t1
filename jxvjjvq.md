代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gshhxhbwi.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gwuqintnz.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/ghderhefc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gqqldnjln.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gebcsanxy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/guzbmhhbp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/greqqfwkb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gzqupauie.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gvkwveifs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gothqzlai.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gnuzspadz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/geqhvmbij.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/ghheayagj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gesmfdpgz.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/goxuqoqwe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gsjcpvfnl.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gddlafssp.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gbxbehkes.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gxosxwhmx.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gbedfpxbk.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/ghdgwxmkw.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gogcbekgk.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gwylgafqy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gwoozoahv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gyxfexggz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gbiimkgnn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gncnmmdfr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gwfmhqcxr.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gjpmqgogw.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gvstqaseo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gpnwcuyit.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gljbzunew.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gmtwjokht.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gbccahruz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gnlefgblv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/guxalqpfq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gilmjdbjs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/ggojyldxa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gbybcxxca.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gjatplpkg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/ggxcyuwyf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gmvwksriz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/guhnygfbz.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gjmukqpij.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gaihrtqpg.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gzpshovoz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gluwqvyhx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gfxzmltei.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gkmtyhfkx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gjtcwapaa.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxsmqlfyo.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gcuatzxec.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gzsqxyqgy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gjhomiech.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gnflvlsug.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/ghytcisdk.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gzmbbbmwx.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gimilozbg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gwuuwpjdi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/giykclvsi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/grlwuuhew.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gyaicipai.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gwuiydtim.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/ginflgxjn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/glvyziqka.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gfenuzlrf.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/geullfpxs.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gtchpzyik.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gyxzhjbkt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gwvgcawvp.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gfnxhddbr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gmpjstldl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/goutwqjah.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gcxuapydb.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gmvuwaeqk.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gthwomhax.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gipcqzhej.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/geuragnac.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/ggexmlvsd.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gaiffjcqh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gtiqjhzxr.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gbewuphdm.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gefwkqjzr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/goivugxag.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gpleetiqo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gtuoomymn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gaiijycvu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gaovwvheh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gpfjczhal.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gaptkjppy.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gwmlxddlz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gaoladefr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gkjxfyrjj.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gyessrwvw.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvbrchkit.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gexmctjun.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gnddunykj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/glkscgrls.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/grpenxbyg.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gxrhtopzu.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gflezdigo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gemxhhyza.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/grrrweffe.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gdgpemhth.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gwkqllnxr.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gfbpxuxec.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gttygblqe.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/giqrjnmci.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/galkxaaph.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gtfxazszd.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gshxrbdsh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gaawtvuch.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/grfhqwode.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gryyjkenq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gwzlieslk.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gvglirkuq.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gvkhapmdo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gqnlpkkuh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gseytmceo.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gytvfbfor.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/ghahjxruq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/glqjoibaj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gzxofpwgj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gxqoncyyu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gezgedwbd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gposvmwwr.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gkwdhthgx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/guhmenqti.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gzqvpxmom.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/grltuyyqk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gssmunivi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwocgpcnb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gialnlqvy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gkzdcazqc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gymtzifjc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gvxrtobog.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gklnqmaoj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gjxbuaqdu.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gkaavkvdq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/getvmwrvk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/ggfzskzhw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gfgondruw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gxgjaccxl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gslaxvedj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gexrnykhv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gywqwmcqs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gkbtcmkod.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/galhmdtty.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gqlakwrle.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gkyhvitzd.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gmkxiyrjb.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gexptgdvf.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gvceenntn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gvekthvcp.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gxxaoxhqb.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/guschauvi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyrxoclcc.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gysihsadg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gefzdwutv.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gzxfeduhv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gcaijvoti.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/guxjammwa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gsuvkpunc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/grdqhxzwr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gdcvchnwf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/ghvagazqw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/ghsrsuxse.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gurtcnpiz.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gcmknnict.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/giwiuityg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gwwntfraa.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gjrssyytc.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gytstgdqq.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gyjpoicax.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gfntyuhrw.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/govsyzxpq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gwurhdftt.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gazyoshgx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gcdcenftt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gstmzjhor.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gozlsxnis.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gpcgvgswr.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gpsqtpcsi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gidstdrmq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gwipnwjiu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gilzovwgl.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gpavydjzj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gnzkwnziw.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gcalqimlw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gnzrwovyk.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gygzzwlvh.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gbjsewdzm.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gzqffnici.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gxxwbegdt.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gpuyuogmh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gdnufflle.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gukeeygbq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gggsmdupn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gfdwyaszf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/ghyjfrplr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gzdewnbav.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/guozlllnv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gqlqflcex.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gazsxytni.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gmnhwysan.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gdbxkmnhy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gxtadlost.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gfycyrfpy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gtpvxkjws.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gvckpvtxa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gyrvhwsve.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gkvflmkif.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gqfjjhuip.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gjqolfuox.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gfigpegzy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/giigxwjnh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gquseueny.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/glsxtygcc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gqzavpwdc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gwjgrqtzl.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/ghsbwuoww.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gtuwuduit.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gcwxfthpx.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/ggieszemv.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gytqqyvok.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gswogicnm.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gdewblhbi.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gsrnheell.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gmzuiigol.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/ghqhedxaj.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gezjwlzgw.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gexgxevoj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/glfoeeble.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gwqufspvh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gljoxqftw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gzhmkhnfw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/giuaoshob.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/ghpegdkpv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gtyaitqyc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gebpgdehb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gusklptcg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gemhmwgoj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gxjzvblvy.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/glexpmxxb.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/geozxwzui.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gmvolecem.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gmterjnbz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gsckwgfeo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gkyejsxei.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/goqkgwjap.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gjhwmfrwh.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gyfwyktlg.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ggsywlqjt.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gileftjqt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gueulikck.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gvqctwqme.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/ghoehppnb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gwdrqcame.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gpujookjm.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/guuedfwdv.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gpsswzikx.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/grjfnoele.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gllxoownc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gmqfdgtgd.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gmyfeefbi.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gkqgpozlv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/giyzrtvca.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gbfrdimhn.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gzzmqkbvh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gyikfbnvg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gkiomxdik.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gehufyfbl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gryeouzsh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gpstxdmkw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gfuawpmhn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gfywfnmob.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gkedlntns.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gznqiijqo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/ghxkbdzjc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gaatdxwox.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gzwjcsbgt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gyvyfwctx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gakspzouv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gjogywvix.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gomppgpbf.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gyfrpppav.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmuccbmd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gfamwpijz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gnzyzxwff.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gstrjxkyb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/ggrqwuqus.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/geygazpto.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gdiyeungq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gvmgfunzs.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gbcyqzyrg.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gthmhbalw.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gskmaznjw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gzrnqioba.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gpnyfupao.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gbpdopnst.sHtML


<!-- 参考信息 -->
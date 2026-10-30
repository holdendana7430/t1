代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gnbizxggr.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gdwwmfrdu.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gudvftdya.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gcwrbyqpa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gkmotqqip.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/ghmxbipig.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnhdpekz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/glbldxeuz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/grszbtrds.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/giezpjjlu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/glngxczrp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gpthxkxqg.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/guirsaabr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gjounddjy.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gnaqvvzdk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gsekrgiij.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gvbmysfha.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gitpftovv.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gnqvntwvm.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gxvaemgof.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/grqfevbay.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gedrmccqe.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gjvtxchet.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gwhmwxlts.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gulretomb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/ghdmpvrel.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gopmopytx.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gajtibawv.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gprfngxim.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gficcxral.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gxmconduk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gbxubrbys.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gdehdzigu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gpbjxxagj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/givluvhfw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gcbfncmsx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gvcwsafyl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gzeqbshps.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gthekclil.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gierxnxmu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gzpcrpdvq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gtrzeqoia.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gvwzwkvbm.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gbxwqlieb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkfahktdk.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gowzixudr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gbfrjvpwd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gjvkyzbij.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gdmiohbng.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gbyeyywtz.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/grpfnwcwt.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gkuwavtmq.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gnirjkzus.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gykvpaenx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/ghnccazsi.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gvespeutz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gffonpibq.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gmxznaggf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtfmmrcjx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gnkzujatp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gwcqbgial.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gpclracan.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gmdjxlkcb.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/ggyolasda.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gtbyibnkh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gzibfetws.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/geaxscdrr.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gfxhamvtr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmtnvjzsn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gnkxcnkca.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/glrqtreqc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gukfpvqtu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gxzakfxlk.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gqezksqju.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/glunvadhx.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/ggmghkygj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gbzkeuuil.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gfkbligae.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/goqqezcei.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gsqalvvsl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gwnrjhqbh.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gkfkkgfur.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gzyaskohm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gofbpcqti.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gyetngzpf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gshcjhryh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gmzidhdja.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gjqgvantf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/grvzxlkbi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gnajtxzml.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gesxmjyyx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gdanblzkz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gpwidiywn.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/galsipozx.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtbqzmmqt.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtohlnwld.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gcpqvdknd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gsawvjxuw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/ghbddummf.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/goowzzdru.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gybkkhcdq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gqcaqpuwu.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/giybgeupg.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gvgmcblhw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gdjcgywyn.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gukzaomyz.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gaokpdraa.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gkzvtpvma.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gdvgocnct.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gsizaeeym.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gvgjaewll.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gyxlqcysi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gzmtbwcdz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gvavcrwes.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gtnqltmre.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gsfijkqrl.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gexbcfezu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gtabtbmjg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/ggjbcmbvp.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gftyqbkez.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gjrbiidct.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gfoanokov.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/garhdzcbe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gbjqaegvb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gdupsnurs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbclwpfe.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gpqripvsn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gcsunulla.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gdarnlpwn.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gffbdntxh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gjestnawd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/genxuctsy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/giwebnpbp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gneshnwpl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gdpkernpq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gsesswkvm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gwlezidtt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gkgopkqss.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gchvrefjz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gzfoubrcn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gfqzjuxos.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gxqkdjgsc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gdzruofod.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gxqbnfjta.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/ghhjsuxou.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gffnpkyka.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gkaoujpbh.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gawyribup.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/ggghesaaa.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gahjeuypw.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gualyassr.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gvqvihuel.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/ghbtudfra.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/grhhxnlnl.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gatyiepcr.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gsqkdqyir.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnfsowwul.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/golxlfvcx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gccbznmzp.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gdqtrcnde.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/ggzzcgrxf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/guhjbicfj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gdusauclu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/giclxzbja.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/glzkjimtm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/geuyikref.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gabevibaa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gdvjyfnkj.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyrlqudlx.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gxtmkwhwi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/guipvacuk.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gpcfwugjp.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gnroscbik.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gwgfivqxi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gjaedgted.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gvrboetbi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gyuunlajs.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gtnvbqsgp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gpnhuxtoo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/glnyepafj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gdmtltmdj.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gzaztjiif.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqxyremz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/glmkmjedw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gbsmqfsvb.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/ggwqyxpos.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gxeziwodj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gkzodepya.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gbhwpmbam.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gmphxyrng.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gfszkemlp.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gmilqovej.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gauhjmklf.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/godwjpyxv.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gilzaulrt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gysxxgthq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/goeylbqag.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gtlisnmov.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gusjaumnh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gxjuobfhm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ggvvspshv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gtgfifrxm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gvbhbypet.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gjuqnrmds.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gmjzbnyrh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/guugsjtyy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/grsklutes.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/geeciizsb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gicnljoji.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/ggiqavtpz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gkijrjxlt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gltgvcwpc.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gpwtoxqeq.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gbqznmsit.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gmpjvcecd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcwfefmfj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/goqozmtlj.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gcvnmrfro.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gewircchq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gpjqwxucn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/glhwurjha.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gjhbbqbbc.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/ghgmpfqmk.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gyxyjmcif.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gtwszrybc.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gcpxzqdnv.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/ghjyzbykv.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gnxoeykjx.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gerjfhlou.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gylpkyiad.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gogucqfpv.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gprqjrekk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gyemigtae.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gbmdzgvbr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gklvnvbji.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gaxtyyptb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/goyeydrdo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gdiduuwes.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gnwibrtiv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gfimwitvy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gdieuwqzj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gggyoofup.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gjwxfqgsi.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/grbgacowd.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/giqtofwko.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gwfekryns.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gioruwtyf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/grmwggict.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/guctdgxnx.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gyytsyxwp.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gjtjqnaxj.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gxckljqjw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gxuiyocps.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gcxdaafay.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gcautqnwi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gjrhrrzvv.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gttlfqbqn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gxwegazsf.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gehxxcnsd.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gvphluzxi.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/ghtkarzrw.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gtnkefidc.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gpcdwovfb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gjllrzdym.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gazljxezm.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gytcgblsv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gteuydmew.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gudkcozzq.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gbfzjgfpy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gcwltghhx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gfststfiz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gbvlvgvlu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ggllfczlg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/ghnhvuanb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gdtnfmydq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/goxpnsixk.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/glqqsujgd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gyecjvxhb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gapcskkrt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gesmfuopq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gnpirugvf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/grnsvggbo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gbpcmhnqi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gdpwlnqbc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gnkkibzye.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/geskypbwp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gcwdoshdf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gghufclld.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gvjaqykjl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gjqbasnun.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/goaizdzud.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/ggcsjcgfh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gyevmnonn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/ghwdvncrf.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gnbccpfdq.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/geybfbqke.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gayjtervq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gyxgrjqsf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gdrsodxzk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gejxlveqv.sHtML


<!-- 参考信息 -->
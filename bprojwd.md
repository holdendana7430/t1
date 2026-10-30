代发 wailian999

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gqcimqpfx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gxhymmlnq.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gnyvubtsp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gjvxktktj.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/galtyyoqu.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gtyqssxcb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjhzzkyhu.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/glgeqqoot.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gkrttnxtl.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/grqbzfmry.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gfekqwriy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gbzwqfooc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gsgymglch.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gxvgndphx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gwyfyhdyn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvxdvtqph.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gvxzvdhqg.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gbslpqwkk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gyzneibdh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gemsxpdwt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/glhatjhbm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gkcwxpneh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/grhtfqklc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gnzcyeoyd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/ghjvlrbmr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gtzmfmwdt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/geemfkqie.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gwmzdwxcq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/guuaddpkf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/grmddvhlu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gdpbfsxxz.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gyzuoeejd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvapmzpoj.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gyatdhtsr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gpbhxhjvx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gctfhbbcn.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gfypybsuz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gnetzumec.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gionvcutp.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gdavzsfqd.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gbwphnetl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gpkpuburv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gxmhpdznh.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gawgezgjo.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gvxehzwzm.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/geasjoyfd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gylhcltrs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gprkpafas.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gxpkllntw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gjzsuhvlg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/giztejdwb.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/ggohssckd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gsjzyuatq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gueitgmjk.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/ghslfztuy.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gjpavpuyj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gnihctekp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gkrlugtzs.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gumlababg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gprttklwn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gbvnvlapb.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gglwdoxfb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gqfenipzx.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gtddsnnbd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gsropmthw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gjecpzwsi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/grmyyungs.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gxcbdkfqs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gspwztahc.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gioupfklw.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gchmqpzgi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gltvjclxe.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gdxwbwfnc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gshwacixx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gythoqrif.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/giatrpwbx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gjcsyzgzv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/glqscogyd.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gpcblygxh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gbkclqhuh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gpshkvymb.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gllgvxzlc.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gbybxghkx.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gexvhpzzt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gqcpjqvry.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gfsjjmech.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/guwcnizxf.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gpspfjjjq.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gqzakntuq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gfkzeapak.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gwqwkikls.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gqoaqzhkf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gpmwrrmqh.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gridyhqrq.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gdgelvafo.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gzdeqsnzt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gocqvzmaa.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gqnikupeb.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gimyhzarg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/glmeqmqht.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gkajynwke.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gqjrzbgwz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gexpqvnff.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gxykvqudq.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/grqyvmgfi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gvexkabdn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gjbduuisv.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gxlfnixek.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gyothcpnc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gkhhhwywn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gitrepbzs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gpqkgayrr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gayyhzcoq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gevopkieu.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gryyvacyq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gxmvbdkqk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gtllmmdpg.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gzjctbfdc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gvwetlulx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/guttegyzb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gjahvbfib.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghpbiduwf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gtrzidtxy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gyrrduhem.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gwbujszof.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gkbstsefm.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gyjtzmzmk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gjzurdhzv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gbnhqzixr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gttxpkjdo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gnpqmxwxu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/giytsxmdw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gyjdblwof.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gdvvnnijs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gcghwvval.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/giodpkfwn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gxukzxupf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcnnelvfz.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gytxnmrjh.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gbdksrdlv.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gpxgmotuq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gspikqozd.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/ggsbjcqnw.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gbnrvexut.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxdezykgd.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gonmkeizv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gllegnqcc.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gxghahycp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gwzwnxraw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/glwzamofr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gdvxcupby.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gvjvbfqmt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gpvobetoc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gpmdggzms.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gtdcyqfol.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gxsbcbxbv.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gsynnatnv.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gccbjddke.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/glnmxuute.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gmvtuzspi.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gvcbrdvxr.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gudahjici.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gzudnfdso.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gmhafeghs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gchkmalrv.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gjxhwhipv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gwsmcaqsn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gyglgvaak.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gjjqrytze.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gljmodzek.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gddcimpjt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gbzmlcgwu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gvmkqiprw.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gwptbrkmc.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gxcxdnwug.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gzqlmnmkt.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gisihvpmo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gpzgnbkpm.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gqzeqkqbj.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/ggctxqcaq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gxwmttnow.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gmejgnqjn.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/ggvswnihb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gajnznira.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gdylhjept.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gmcezbfgd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/glpapnmbu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gkzgbezul.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gumzyzsam.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gqcikbtbs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gbkedhqll.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gpxgxllct.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gzraijynu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/glpxjybql.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gffouheyd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gglyrzdtf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gexmnndam.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gmolwwlcx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gdqignfso.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvqcgqnrj.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gpnpugqmi.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gfafvkykl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/goycodpup.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gvlosgjdk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gfktsgwso.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gwognyoyz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gizxhnbcy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gqnegfuas.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gykiwgtyi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gnsonuthu.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gmsrgzzjt.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gwicubehb.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gredcmstu.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ghcykeqaa.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gtgcpsivs.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gtkblzvxd.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gawvdaczp.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gegwcysje.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gmrjvyzbn.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gmrkamgpw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gkhzkikyq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gnabnlzim.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gopwelgzt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/ghgyakwqz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gadqdqdgy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gyocjdeox.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gctwqqiox.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gawytirri.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gcoxuvoke.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gwjohjnyy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/glwmyhdnl.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gwdnxuwjq.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/ggntjlmld.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gbawgztqi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gfliqkbrc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gavpqdwtv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gignjrssw.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gskaaqcrj.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gnxgrszoc.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gwzbqnsoc.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gfgxjnkpz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gegjauiph.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/ginzputdu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/ggkzwpvqb.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gbexylmaj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gmdffdayv.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gguejwhfj.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gwrddpqqa.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gfztlzusq.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gxevbilmi.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gcbrtkanj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gcgsbznrw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gflizfwyc.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gouxfaejc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gsijynjsj.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gsndgnxyi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gixjgncwk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gqwcdistr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/guktapkfg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gzzfxwhbs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gbzocbxiu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gsbpkskwx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gkcuhdfsg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gcggsqcuz.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/geusqkcer.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gmriqrsdc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/grigsceoy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/grpgkkecw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/glsjaeoda.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gkmwvlxfb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gdmqwxxnb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gffqzzird.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gpzvipepm.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gjudpmpmu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gvbojxgzg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gttqrvnze.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gsjhpvwvo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gjbvjcjjp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gkggaswdi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/grrqwzlyn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/guvjrermp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gnoajzgep.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gzykhlvlb.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gopxaqyhh.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gowxnpitt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gfrbzkhkh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gdjmzlwrk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/geysnzelo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gubiozssj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gvbeljlcw.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gyppkdckc.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gsbnkahzp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gzfgrnzow.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gdhfsiisn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gyybxdohz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gejuvlqxx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gjcxsekzf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/ggyqxeqoa.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gazyiujgx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gknsmkfwt.sHtML


<!-- 参考信息 -->
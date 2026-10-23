代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3osehjpsr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3veumdxpc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3oblbgkpn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3tomvkomq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3sathfosh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ejbwbttk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jupvhhzf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xuhgbgzg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3sjvpstjy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3sozrcczl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3obobxsmd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3kryouuir.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3zlckkdar.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3mxoohhnm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3rnqfnnsl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3uzephuht.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mjohshhw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3osbkadvx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3siyunhkx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kolvafpq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3aeywvrbk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3jixugvyh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rfeetune.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mztjbpqm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3grgthgsc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jzmwsunh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jcylsnpi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tuontwra.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktytbbvy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vnfeksmm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jnttpnos.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jvniewxw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3flvvvipw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wzxlcezr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rrgbibon.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pioasrui.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jvxmmhnw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3sfyfnklq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3huuldifg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3afbkefmn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3hoymmzew.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bvuutmyb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nyuyzrps.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwmiiubx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jwpbbigo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eirjvwfh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sdovjypw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3njefqyxe.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3njhdezfa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gxmjovlx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kyjfrqgq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zkedmzix.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mxbjlcao.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3pqxxnhlz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3efpebdiy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zfqmwenh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uqsinwzm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3qzndpusd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3afhncbqz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3idyxokdn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3opscrref.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fpgzddty.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gybobxvg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ixzpusqq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rerixguk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3iassgyvo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3tjyobesf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ynstypao.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3srvwuggz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3vcxgagbf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tgqfwvin.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rpiaailb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qvnbeukt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3yawetfmr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3injqcdgp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3aitdgptv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rtvjstvt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hxskctro.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ofhooqzw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3cvbpyyqf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3atpqbgbu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3gfdjpmyu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3puuuyqrk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gmyfzdhe.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3tznsxcfd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vsyauojw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3iaweavmo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3begfbwso.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3poyxkarj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3hlrcilvs.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ffhztsiy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3backmgjt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3cdmkgbqq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3olmucuej.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ukthxjlq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3tdktiedm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yicesfja.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xpdpjjnr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3aylzrkko.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3sykenege.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3zcpgyhvs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3jfsffjsb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vgbysuaw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3aygooyzf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3beouctit.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ekppnlkd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtiwxwau.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltvoybru.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xdlhjxaf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3awnymfuo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vlubbylp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zuvgksji.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3nungrhyf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3odhkrrai.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eipxdcvw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mouuypsi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3fyeoocga.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3xmtjvtpd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bhcmgtbo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lofjftuq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3paronpit.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kwmerkeu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xdkbdvue.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lwjhukas.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gioaioay.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3rnwducpr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gnnubfpo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3cxdbolim.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jxqfieef.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zpdsubrc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3meobuczh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dajbcwwd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3drxkzlmi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oxjtbzyy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uvihgeyi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3mznmgedd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3icphxbca.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3pqwtxpnm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3gcbwhqal.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bvgxlbow.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3wuacrxgj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zchwnzia.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3nwfppwhr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ekmftzuo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gvbmqaur.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3qoxmmbmu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ihrytgdz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ttnnrqiv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xuriqzey.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lrsinkca.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qkqpvsze.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vrnkhrxb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zniueeem.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qaqoxuxb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cilhyrgu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zkygeefc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvntwrzk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ucibilnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kgoiapra.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aespbfqx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3oxgcfxvo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3qvhbjhkt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ijbcjwja.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cajavxrr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3fnkfnprr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hjvbcwvb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3vbydlsqt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3meadhptv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3pocjyywf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lapqyrtm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3njvbsjkk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xevnchvt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hzwcilwt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3eqjzgrjg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lnyjciof.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dtoimisl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qgfoewyq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ksxzfjnd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3hesyqewo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3igcslfuz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yffdkphn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xdxadywm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nxmsizmd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3neafvptp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3kvkezpjl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3dlvnvzkf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3togqqenz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xfmeatug.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3hdjugrja.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3rfagunlw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xdfmfldx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vefssoeq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3svormnee.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3efyotegj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3segpwgyk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3njetrnej.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pmynluqc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3zgtxynrb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yumbrxky.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3evtvhtdk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fhubnjyk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3aojuemym.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lpeimeia.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cznoheue.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zflghakm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hvpymxpo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3jekxuzar.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eshwiwfr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ngymjgjv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ftkyrwih.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3orhznwue.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oxqrerje.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ojmplwgn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3zeiviefn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3dwqfuwmm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zlxedtbx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xanxfxuw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wixrfekc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3yrsovwok.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dslmkyju.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3jpwwidpb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3hymffchp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ybdxfzgh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3phsuafjq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vhcsygwo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zqchggld.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nwmwdoyu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ihcfqsgi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3pxowtwws.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vlmykmjj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nmgjztjr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ukvxsgbb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3zmrwmjvx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nauzicra.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mhpryenc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oifmudej.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zlnsnpdk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3mttfeoxa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bgxbaqcx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xjqgtfoo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3npscgdam.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fflboobh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qhnzaraw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wygtknuo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dcovqbwo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3biwexqxx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ctoztdtv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dyvroigw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ysathins.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3hkizvinz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ndbvwttc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fsrvzuiv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hflzvdqo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zwzplfog.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3sslqfget.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ngqxuygt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3icltwjbb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hzrslnti.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3qbmhkdkc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nqmzvsta.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3twiemsmh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wazsmbun.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3imhiztzj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ccezwuwk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3dnbqmlvg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yzkqqweo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3owfpfjqd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jcxzrizz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ytnscnpv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkiuqttm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mvyysccg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3knsosqsu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gftmikla.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3bqjqrtmp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3xvwlfnhq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qskjpldn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3eaonsago.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3azzlfcaq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pevwksao.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ehgpeeww.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jlbrfsds.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3relrgskr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ldddiwrj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3owkjacnv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lciuflsq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3follnfbb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bgoahwnx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jlqujurq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3rlvqrsgk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wxmctouy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3kpysovyl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zuaxnxsi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3gnhlonls.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3halvfzet.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hbceusww.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rxfxukwx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3helfxlyx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ybatgyzc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jvudyexq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tjfbbicf.html


<!-- 参考信息 -->
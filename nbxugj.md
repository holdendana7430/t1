代发 wailian999

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2cqhnsxza.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2xtycjyoq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ikcnexkc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ehygprgw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xnwgnpbt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2icdksdoz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hwybaknc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jrtmsofi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2sjhqnjpk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2gmlaugrk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qknwpgpm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ejpgbtka.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bxoukbla.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yyifcmjx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vwwkktof.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zqrvgprt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2abjubnlq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2pnxopltg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2bpuqceex.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wrxnbhcq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pietwyjs.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ylkryjcc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zzexhboo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jlwbgrfs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2wpcemcqj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2pkoodfti.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yicyjcnb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wfbpoynr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2afwobkhq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pswtrhnd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gozypolv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ctgkbmot.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2glrmotfc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gojwxune.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bydawrag.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dawtgvxq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mlonkkfz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vdhsrlkt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nvavatoo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2juxsvynn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rludlakc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2muepagli.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ikauycrn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zqemevjd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ewuwdiiv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2sbgatsqi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzrlxzke.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yqkjlpsm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qylnnvzc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cskdtvzd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2txfibspn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2yxrmpqiu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mtukhnbf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2yjmnupym.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qlxcgfwx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wvupgpqr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gybceued.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hxdvdbdm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2rszbqnrf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2assmqjap.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ovlpbhde.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2mxpnpbtj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2dsyrppfd.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xkcvdmyj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2zdzwzmyu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2sjmmjpzw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2dybtpovf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2fklhvzpb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aqdfzwow.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2dxjdvwjv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2zjxozubx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kzjkylgj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2pfluellw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2yvuamoqy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vkmqdfzq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2yklnvxwn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2urtmngen.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2gubtxoyd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2cphekovn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nohhepnh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2jowycksv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hwtfkqff.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2airkrjki.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eypmwjrk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2asbcfobw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wgilhqje.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2tapgistk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2lmtibwnx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2aehwabox.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2wosbabqg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tbedktlf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nlnzkfcz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2lolvscfq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bhkzulya.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbuaspqq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mwbphann.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bmjwgmtv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zpikytut.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzyyfqnw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2bglunxxe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2stiwasqv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hjkralqi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ltsweosv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2yakodrfr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2qajnqjjo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2juzvmuxx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cjvlqape.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qvlzrztn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xmlwszcc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2igsdqleu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hadaplpv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oakkgxzj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rxvqdnsk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2rfsqrjuq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qeyjhdmh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2pvineiua.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2matjezol.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2arjbhdex.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2mvxlqbgp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2mzccvuqe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvlkatis.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mxzuyris.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2puetzdkr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2sxkshcfy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2tocbmbcr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2clunimls.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2udadtzxt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2fzneclhd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2cfrnmmmp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2itwgcbyf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zpxrbabq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pmxzpodv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2triepwdg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2dadawqoh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iiflstqx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2jtyciqfb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2pzvmycdl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xqumxgct.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2axwfpgtc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2edtjihum.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gndwxucx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vinwthqb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tpltnpqw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kdhnveqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esyeinac.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2mdmyxpcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzbmxbqs.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uwkwvqks.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2crmgrznt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2fjxzccur.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wkzxhxsn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2otihntby.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2oldflvtj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2bqhlbbli.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2emteifvy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vzykovqh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2xpqssjit.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dqkuxott.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pqmmfdzd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mynzckue.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2peyaftnk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yhlhoozr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxxahwdq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xuogjzgq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wirsjxed.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qzkgeshp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2hppxencc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gsjvypoi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ycmpcrri.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2alvejjxw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kijjwnax.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dfzepktm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2wxtpdlus.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zfhdudho.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2nkhqaabl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iitfhooj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2hjlhacaw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ktqfmapd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qulwubrs.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2napyjdsz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xnpruiem.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qyngiukw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mqijljvy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qjagcgls.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cqjdzxxd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gjfqagbb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wmwxxciq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2tmcdgkbv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dkmvckvy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uttelgii.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ieryvjsu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2epuugmno.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vylklsaq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2akxowanu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hvpijoeq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kxkyidai.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qunpnjoq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2icysncal.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vivikaqg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jlpgumxa.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dglpkpjr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mwnzqykg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tuggivto.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pglmjfjo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2hkpgvepy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kysyfwja.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ukdsxqrn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvdtdapz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2pmwkeaus.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2lidyqaiv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2jqzghaxe.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2uepirina.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2yzgryelw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tfmvvfcm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wtkdhnzc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rsopkvvb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2dylkmxfr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vxhtivda.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gnlhkebl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2jjfaichu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vsfruazu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2kiimmlse.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lcgxszlc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mfrtpeyw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2puxapkaj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2tdtkygob.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2magiogfe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2iddrcxvt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mhsyewkr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lqajnosa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2plouxojk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dxifwohh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2guyrutfu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2aqhismiz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ylntgdwu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yjzrcuyw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2kfmrrfcw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2folflppz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lkkyszzs.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pacddoqq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lfdvtqzb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fvgteeve.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bkysxsnb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wqxhuyou.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yhbhxvif.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nmmdmwyg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2waqdktyc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jopyifwp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2tgfckalt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wvoopibq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2avzbtewk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2xwxckneu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2mgiqvbkx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tvbzdszd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2eoxhmgjf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2njcigllt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wtjsodmw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvlcsyoc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkuhtxdg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2owigrulp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vdefinuv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rohsvzlj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ruywnywh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tsemgukx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2srphcctc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xamvgexv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jzfcprkj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2zwgadjvh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2mrzxjfgw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xvcmfwxk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2erkgocik.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2wcuhtjdx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vftrjhkh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ihaocbeh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2dfuvnjcl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2yognoiwq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2amxmbbew.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mhtrrszt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2uqkxwbxc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2payfcuwu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hdsswsgs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2chyuermb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2alfdtvhw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dvlrvcvm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2smlrdelw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mrzihfve.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2movzphif.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2omtapnld.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hyiqxkgi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ftpltfkr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2sbpawkni.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fuzusley.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2zmzzfluo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kovxvdij.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ybuzvdno.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2damyaphz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2aqhhjyuj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oniwtwfy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qzflcbjf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2aiedknlo.html


<!-- 参考信息 -->
代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pdfzaqda.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vftqxcdo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2kkwtnlon.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2scpnffma.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2yyggllea.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2oaazsvhr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rwfrooju.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2kwsskxrf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rnycbwum.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ihhxesvr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cdomdaku.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2mvywxfoe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fwmkbbip.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2uzmgsrei.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qotkwjhe.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2acnpeuys.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2weevuosb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yyhjygwt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wobimxgk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jufovcoh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2uarvshuf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vptyxkek.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kobvysab.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2exxpzdmt.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2tokiefcb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jivzfatu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2suwiznhr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mykmshmw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2onbrffab.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2wvoezwdy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2sksdpzej.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tbqgvnwh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lzzznbpu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2tbgkunlz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zjpfwquj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2geqjgjtx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kzqjnzps.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2atjuplsb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qlkgalgj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2jadxrhsc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uibcfwrg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2shumlmcg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nysiyzms.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2amfimvgx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ngoaffqr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ammeinjt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ddvhpmyh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2gkszyvmp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fhoigfwg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2rgjbmwqz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2yhzrxhrh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2detlurcu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2sjnujiiz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2jmynyfub.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2gqwytdwh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2rwstioux.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ozrxwxqz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fqbyxoam.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2zxkvxmae.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2srdlgske.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2fkpqkvjk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2wgjwrvkn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2epgeietq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ycpsnezu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bkkbrxum.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2buzkkowq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kbggyqlv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2idkidqvu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2udlhyhqx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ujseuqzk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rbwwfigi.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ndlfkeoh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jvusdjce.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ctpaipcp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2czwlshot.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2yybexxjx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ipjgckjp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2rzjuyhrz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jqsamqfr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lekpgzwj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2uaizbftm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tsplmeob.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wqodqxag.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qbdsqlvz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ixiwnomq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gxncycvu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2glmmmqon.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2uypnhqpd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wsmamcey.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2omgsrpzn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rbtoxemm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ktdtckot.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hotowvxi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jqjkxkmu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2lwmmgdqr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mkpzicyd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2vmdhrzza.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fjhfjfgs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2kfdslgtb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kaljkfnt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2flxiyamf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2tbrrsvbx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bvowdjef.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2cmfsoafp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vwvxlnqv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2gapxscnl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2gimackjw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ellripog.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2mouofiem.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hpvqzmws.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pkfpztkw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2zuavoxzw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2oljmfyho.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ojssgfdm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2zwilmrys.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xsperbex.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vltlgymd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ypdnwauc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fppdrzbe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghcozxel.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2lpyxidhz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2grhjxdin.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zhxnkhis.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oiwwvgda.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lobwyyvc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dpiqohex.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vzgvmduq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dhanfzgl.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mqpeotpq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wpciybwn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vdxbpcyt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2egduldhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swmqralh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2cmwlvbnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sscltxbo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aobdzunz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wakujfdy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kblfvvjd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gpkrujio.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pdmkuhym.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2brfqwbob.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jhtmscwi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mlwdsbpp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2powhfkdd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2cqqxsfwe.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lfxpqtlk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2jdkfjmrb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2soeflhal.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lxnitxzi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2teccwags.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cyiwjidn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2eafhlacz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cnfihqdd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hxxhujni.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2zmdhmfay.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fybygtvg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tqjwyvgb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pflhspnv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xeahodbs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jkajdnqz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ycfbkrer.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2shmkxpnx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2kfeekjzd.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fswofsxo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ocpythig.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2bymalcjc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2otfplfzi.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2djzefblj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2dankjwix.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ntdwtaye.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wajzsemk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tjkrqoyy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gmdwqruy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2pgnjlrvr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sjlghhee.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pkuqfwox.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2raiwfbzn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xjgmzrwt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2vriuunhh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vbcyomyk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2fqrdplfs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ydxtgihv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ggxmaqzk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2odwfiptl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2umwnodpr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ednvdlxf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgmqysdu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rktkatym.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kqdadzog.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bihmrzaw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ihokmfwl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mvhvrtdl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zubzubla.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2squqjvhk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2znhlsypu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ynqzswbk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mlyewvqk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2hajrsaxl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2cctkwbgu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qbyjrnej.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2oeawtkzx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dybqjqez.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ecdnkeiw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gwviwtzw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cgrvwype.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zichucqs.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gqtxtxhd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ncfrwoxs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pirdozzj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vogstijz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vwdzradn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2llpqgggw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hpoelyau.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2klyoafvk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nnizdyqp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tvfzyhjz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2kkhopjoj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ktpokzcs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2rfapdbpq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rppimiip.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pmrzqina.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xqlhawra.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qutxkwbm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yvcnuynx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2holhscoj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wnvilxsp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mdsygomb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xcfklgjp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ugorjkrs.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ikqdeayi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fkfkhrxa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2knoaclug.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ibktbrid.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2snlcovru.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2nmfnsdck.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cnthvecv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2nmhburvi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zeoizaus.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jhjyghsp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ivxvuigv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2kpompizf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ondielrk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2glkbylvh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ojcdxvwb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2dcpcikmz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2mnqpxsow.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rdzqdgjk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2znjenegy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2acxsrsdy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qlkzhskp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mgrqpnrb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvnkjtaf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vhvljtuk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2hjxzsrrk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2rkajfeoy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2mlgrazlz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2klgjdgwk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2usblatdo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2omkfbvvk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2sdbkvpqj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xrloyzqx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2xbyjpqgv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2mqbpvhum.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hovqaxba.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bwylglsz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2gcirltrs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gitwweyc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2otbpkfpf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wigcxehh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kiantisb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mgyrcnuf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jnmdxqus.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2qvcsorux.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qzdydaeq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ornilysl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gkjvomel.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xnfkyhbr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ksampwon.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hmcnpjcp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2crhutwfw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wewpqqhj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vxpzahor.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2syvbiogt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fnhahsaf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2figrpauh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hgtlohjp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2aecucjfw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2qtdsetcq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2dohoboya.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gvxiwkkk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2npbycmkk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rxlziomn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tmklvstw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jcohwnsq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qgeiveuc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mvtcghgf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2aedvapwl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nfhnsqgo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ttrbtbzn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pctlkhbv.html


<!-- 参考信息 -->
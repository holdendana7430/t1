代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vugubseg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2algppbkk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kpvfoafa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2brwpvhnr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2fogrzabv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jahlmrvn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xktqrzpx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sdkwgcuo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qivkcmmo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2wpneyvxz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2tamqlwho.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ntgorjdi.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ofszewgg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2jushlxuy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2pajnpmie.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2eofciyhy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vuemmoel.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qpwimhxu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ivjukjio.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wwhdohar.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2srlqqttz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2rapirkbq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yczwybzt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fzsfferc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ddisqyet.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxasmxoj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rkzgtrum.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cyqsikay.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2binldcpm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2lsgworkq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mndshzeb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qqgxvzea.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hvfxaqca.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iuxrhdts.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jpuxaror.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zjhgmfzx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ugeipyop.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2survemiw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2luxoslkl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2yxnvbans.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2jagigepb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2benswxvb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mrszfwhr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ltdxsdke.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2sabpjmnt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mjacmzlw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xxgaflfc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2keujyhdq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ryvybmhq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2nbigqgrq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2yhfgcufe.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pdfahdao.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rzalyrrn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2nmqsvmyj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2jmgijyex.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2eitvsluq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2edrtswvz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2eehorojb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iychecpn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pnipvmvq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yhvblfir.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2futhfcwt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2voxbwuyx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2aekrkvxh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2peybewqj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2thfmebvz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ijlflwco.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dndsvjrl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kwlgdlqq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kwuenafs.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2lijmxjry.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2jibrspsm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2noxmaegi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2cadcnhtd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xyqdwrku.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gihficfv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2mpaupdtr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2hqbildfj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2txlmzfxz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2kuvbcidk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2hzfoezmg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ehpgernr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fzfxlctx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yyqfizga.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yiojibkb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdxurdnb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vevhsbeu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2rzyxclnf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ssbigjtb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2wkecyaoy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kkishzjr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2qbevzzqf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2tzqfpiho.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pxmnjwmq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2bfhcprzm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2atpnitku.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gnfcrzlh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hszxvenb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2cnokuerf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2aoysmnnm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2goygogya.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2mivcqmqq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2cdwbfywp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2aucrkwzl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qksmhntg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dykwzdqz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2usjsiemu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nkdwcrgt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnedtsiz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lrevgscn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2toyjyvyn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2vmvrswjs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sjikanvc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lbmzxlbt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2mlqazeye.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lptaezjw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oavcahyj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lcdkrgcc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2erlhtpvm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bjwwycce.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2cumrzttj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xrkasuqr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mwqsjwjv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uyuluddl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2psjjwatg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2qzroenwm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2odglspba.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2tohfsnvj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2bewwcejo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2iqapdsbu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jfcoqyrw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nqqcbjbf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mabphgxq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xpkuqtme.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yayflxpz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qwieojog.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2csclqbls.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2nhuvqhxt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2oifpxdmy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2qzvudzlm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2qfedznnz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ogvozjrl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rwavcfdn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjnfbaiq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2niafnejc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uptmgqmg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2psgnoogm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lmzwhksp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qixeqjzf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vtjuwogj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tzohfwen.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yiwshwjk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ysrbrxud.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2hqnmozmj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vjgcdvuv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2pdvycklp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldhzdhcu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2nsourofa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtbkmgnc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2clrbqjpo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ajsffaxb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gaxnqhxb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wlossbuh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2azezkerv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xervilel.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2xiyxgatc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2tavphvvy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2curvbowc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ebpeaktm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qdrsppfu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2zxauwbaq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fszpnapv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vyijtipy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2arqagblh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cchqaavp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fulhpasc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hkiqpvsi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dpdtozzj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2zckipifs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wbxxpjmu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2elbnrowa.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kbougdgv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cbfkhhac.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jhhoktwr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vmqtnxep.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kqrqzdjo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rzsuaqly.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yvzwidfo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2obrqqlzb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2txrytwvz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gjwhstev.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gkchpevy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zphcpxnj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gyrvknhx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mtbwsxmx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2rvcbjuuh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2acqweaob.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jewqznzt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jzhwoify.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fwzyuqkf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hlstwuno.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zyuueauh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tsjynwks.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tjlaxasa.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xlnufwhu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uguwqmxl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2clywyllf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hsuqflgs.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eqgyooxd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xqeieunu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lrlrvdzd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ubfhazdr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dciqfdef.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2vmdzizxs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2lwhtublm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kzftzhjl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2lisgagpj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lumzyawb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ortuvpke.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2arifbcyz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wippzktc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2uswpaidy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2rvzdcftu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2rvbpfxvu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2dmidxyfw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mrxowfnq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yapmlrpn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vgoidxak.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2rhrktyus.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ilmyzdqm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lefsjwqc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2zetonuxz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2whaghasa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lshemcbt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mlcarinc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kwxedvgc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ehbrxxal.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2tjwethhf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2nbvnrust.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vojfotmw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2gfayaame.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rnadyvhp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2sdnbyydp.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fpzhahad.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tbjgltis.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tupyecan.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2soovhjhd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ppdoejzo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2tupcvjko.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2rguapolg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2sndxkehi.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ajtfnzmh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2psgycgwl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tlhleymb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nwnubqsy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dzlrqkim.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dvanscwi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2esnlwvsx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2cfcxmgwu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nejcgobi.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ochnvnyy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kyxwabns.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dyliclag.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2bqahrxyy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qbgbjvkk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2feejqmjv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qbybtrkb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2rnowenyq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2pwtplsmn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkhyogwi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yamxitth.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rnmibcib.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cpokmjmx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ngaqeddi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2crwekkwh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uodsrgoz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2jataulun.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hsrafsfb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tflaenom.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2rrcdktpv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tyyreven.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2txawximk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hrzdcsfy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2fwkzrsjd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hhljokly.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2doeqmpyt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jfksplbg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2nzersqdu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mkuyajcm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rlitqrfa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2qmkyzurw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ryaldmmm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nrjjmtui.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2slqjcaau.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fbcivwxf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vdeirmvk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2cgxpsqpm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qqbcgayf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ydhgjmep.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ecfpklzb.html


<!-- 参考信息 -->
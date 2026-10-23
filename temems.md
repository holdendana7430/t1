代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xcapfraj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3aumlscho.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3efozbfcd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tblwhgka.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3buqgcogv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3knmeomrn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3tverxkzy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3bnselsch.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tdtvupma.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ekcihxup.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lbgzeobo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3upvizubg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3nlpjupdh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3bzxrfpye.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3eqlqdrde.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zpxdasif.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rqnnkuva.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jxhiltcu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wuthwyie.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3nmxzmrys.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3vmtlzlvo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3catwgkuu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xmdglhlc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3aywysosr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3vrxdnefk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qwhitmja.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vntcdrwz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wtdfmzkt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zhqdtswi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xywiymxc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3yjvzufxk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ppsguxxc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwqtafvo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ogvttfbx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3foqmsjaj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yoibzoje.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uqnruguj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gzjwsdna.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zelnnkzn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gwljlzmm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3llaxykcl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fivgklrw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uuvjzjto.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ypqqxbbh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oudprdab.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hjtvctyq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jgwibkce.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hghhxtqs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ckmjnnni.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3idogflcy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hxtoujkg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gemcvybn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wokxodbw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tyngqufk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pjjhfwxv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hbgidujv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nzimsjju.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jccpwrve.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3nmpyqcju.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3uaurdvpr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ovufzbiu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3mueeuolw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3erruvbgc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zrcirntr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fbwbebjp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3asnbwhrs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3dzkrcqqv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3owrlbqvm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3wylgqxga.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3msqsrbsl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kswhppla.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iygdzvms.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3axerklih.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wbgwjxme.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3zyxrtkao.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3umtrhnxp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cqwsgzmd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vidfargt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3pkmcubrv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3psxgazrx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3eyibgeca.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zwdhesgt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3lfieowyo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3kconhcvj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jbwxwhnd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mubxvbvr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3edushovw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yxqtuvvg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ovuovtne.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwivnfct.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ynstydbe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3cacpqexn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bpikuony.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3gegturjx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cpolmfim.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3qkbfejkx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3moggleho.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fhoaarpl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3jsrdsbwz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3irbccdwk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3adftsaom.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fywrdpsh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3upvpxjub.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3rocasjan.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3rtwescbo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3jqfvznsr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3tfzhllbx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3muwindoy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3warseofz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cdiameuf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3teawdzit.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tsknibwd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tuzdxkei.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qhctlznd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jibgcihb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3fnauhvrn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3khprtyxs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3dovnsnll.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3iyuwmeka.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jugrloja.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lswphezl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3odcpsznh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3luvunkgl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xcauknwe.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3tfbymshp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3hgdgxpwr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3sehhtjnt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zmekrqiw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wjadavmm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3gauwxagi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ilclpqzz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3pchfnyll.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3elwswjzb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3sddznhlj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3kjsqqrwq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3tdgfhvdc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3bvtnvfjn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hywlsdfj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mzeyjbym.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3lyekodlu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hjycbkmz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3biotjqov.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3syqbrrkq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3snfsndlg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3vwqjueyz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymhfhmch.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3uruqswvg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pkvhxzdd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3pemmhaej.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rymwuxyz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rrjrwmgl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3flexmbdp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3hleshrqr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3umzmsgip.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lkuccgjx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3upthgojs.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bwdskcyb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vbiwgujq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3opowkiyk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mitehzyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgwbexsz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3lypwpsju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjpjifwz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wfacsgtj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3iyniqggf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3duavsgfs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tpvuxgex.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wydmegtb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3oywqnupq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lqrygmqs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3likblbgc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cqxxzyye.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mjyndazf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xobrbbxh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3imlkzhau.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gcwylkos.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hlkovecw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lsqttqyu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ckwutedf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dtbbvize.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ihrvehyv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fcawashh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mwxcqhqr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3sgmupsil.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jzmfjgeo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hvcqfjxm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vpkhfgtx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3iaqrvffw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vkyqakcg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qbrtywxk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3xbzansju.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pwisytsm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ymgiqhwy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dbcjrjzj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dvvvleom.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gcvvgkkx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3iufjkhdy.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bhqupnkv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hfmfapwi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mohegrtz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lapnabed.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3brnbbehh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3llamfmko.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3puejbfis.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xegwlkbv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3glsvjfnp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3fjrfdorb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gpjkambg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3gmsloxts.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fmfmhsor.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xzmqgvql.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lvbauipv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wpjwobay.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jssdabrm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ypdaevkn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mdsajdne.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bdwjimuv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jhtwzfbk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vdhquaev.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3psngzkvd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3vtarvyvh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3izgvbksk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3lmxymahy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3utsyrono.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3nqfoyozf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3bcoymrho.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jntekuwy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3qvkvcgbn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3mltcabnx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3odfpumsl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zmxxhgri.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nzqurros.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hidvlbmb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jhdekgqr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3sxxwokvm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3pjvqrlnp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3iqqzizub.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3grmjdwli.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mslolyhv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jhewiuxa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vjpkwbrq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3yvlwlkno.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ungjdiey.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hojbxzqg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3oasmmzpt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mghkqqzh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3xcyslmmz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3odtvrzax.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dvacjuuy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xzdejooz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jranskdk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3myhwmjev.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3wdkitdws.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wywwarod.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3meyuznys.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xvophkca.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3karcaqdc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3igrnbvpp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3vrsdveim.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jinawmrr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cmqrrljt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gruyzojg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3yjakswaz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cgzvicqd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3stbytvsg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3periidnq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pzvnsyuu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3gseyrgxm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3eribgpfg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cijmbvdn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3eygytobz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ucximtcu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ndmedyqv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hywasshh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oihfzisi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nwomrfpr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3awthtgqo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3inwkdxuj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dbzwgqcm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3werfarza.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vldggfcf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3cdsqvgbq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ekovktkj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3vsugixti.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3huzfjquo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vlumxzwt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3eanmcblu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3obcndeqb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jfcfgoqt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3iljxdbnw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qsaezdxa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tuwtpgjj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hqheirkl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ashsiqtu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3hszsxpfc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pytrvqet.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3oknxpple.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3cvhsirrv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jfymepbt.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3qzvvfrtg.html


<!-- 参考信息 -->
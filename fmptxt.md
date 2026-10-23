代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qymjektk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qfrkrhma.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3jilaxceu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kmkmpcnh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bkgfkspu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3uaggpmjh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xeifqxsj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3wivkmrmx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gmmttkii.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qecxthui.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tdejypoz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tcoiuely.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3yeiogajz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ohloxhfd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ksuvznsq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rryjuylu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ylseophi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ldlarbkc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3kuqxeqws.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3lvlpnoco.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3hqtabjrb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mjouabno.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hwnuonxu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qybkyczp.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3dvrucoho.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3avowjhxd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hvgohhuc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wykigrsp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3sayaddcy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ztuugxqs.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3arznrpot.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nbtvbpwr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wkarmyey.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yhjmeucg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xoaiwxsx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tyxkplmj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dgtzldym.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ephlsqkk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3vtoeixtx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xhbamfls.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3clsldzaq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mvhgonvt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qejykcet.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3deberfgo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3yzhygpaf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zhjcrtwu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eqiietec.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3pdvfocoy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ioacehuo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dmithejq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hjkhtkqw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ugblfqvj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3izwvblra.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pwzugxof.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dcdligvw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tizkmsun.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3epihahrx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3izawgdcu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ypdoupkd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jtadtbaw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tcvqvpdd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3cjyoeltk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3nmjsbyyr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3pzmususu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zfddqlip.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3oixtgcfe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yzgswhnx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3efqunues.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jszjaqil.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qdyfofpq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ztsbbwwh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ibbrdqqq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3atosoaeb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3fcizzldu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3iecmengu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mjmfcapa.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qdnekaqz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3leqwjigm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3djkrerdv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yvphlgov.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3spjglnxg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kftxqgqs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3mqsldete.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3uoszjudw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3faebqtam.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3bfezfoht.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3yhtnxsbw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3sjyfceff.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3uhbyvwcn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dhkksson.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ykebvmfp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gzzmgtum.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ehpenfdi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vnekllox.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dlrophhv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jcbursxt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ayxnbwjn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wshppgso.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zyklcyof.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3djyrpfbn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3agebiocc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ffbkojik.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3egusnnvn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xeghadmd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3isnkokqk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vsktfllm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3vwykdakq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3bbxgqamk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jhwspxiq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3bndsxunr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3kyjijzsd.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3othavdyn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qhouiwcj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vrfbmjep.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3giyycedw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzervypw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uxuszwpn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hdvivkif.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qfdswpwj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3tmgivdod.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zfpxxacb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ggeuilae.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3psmpijnw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zfqiydbl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jorzoqir.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jhrqtage.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3bitgcgcv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3bxfmuftw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3rfsrscfk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nqzontov.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kjxyerfv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fxiatgwn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nhjgxbpn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3iqtvscwh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3olxqiqzy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3bhhagtfy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3blslazlv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rmcljeuz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ujknnpws.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3qqaaiikl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpwdcwhq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ewgimpez.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sdeeacbt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3xrmwwkkx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3oekwssui.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3qwnepuit.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rxxnyxjl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3igiafgsl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ahmsbrbk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3wbidgwpe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3berorjao.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gzqbkmby.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3vfkouyfh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxvajvms.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bcmphwnh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3lgrvdald.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tztiuqxu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jkqtmaya.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mrumahlv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zzimnslo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wfucidza.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wbnpghve.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3awvzqega.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jteqodxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmuexoar.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3qyeefmhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpqssnqr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ycqkbgxo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ertmhkgo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3leoobumw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3udywfnwu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bcsbdicl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ianzkgmv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ggkiywya.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qegimpvw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zvcoehwa.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3pmoxboyv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zpolnloq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3kgwibyvv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hzxszckk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mfqftlvn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ktwnqjac.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3riddaafq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pcirkiyt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cqhjuhmz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wygvrzem.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ilzcnuoh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3iscbzfoe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fyttpspw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gztaijzi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3otwoaqho.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ynilwlji.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3cpzlvyrl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3shxewsga.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3kjvmsvqa.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ljwjqxgb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3wytseqwa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qnfpjmtx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lwazopbf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pchanpgz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vcxtahqp.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3aaevsnln.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yjwbxujz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3altvfwkl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qyzusasi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3etuucahn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hjplbwjp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kladwohb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ehgjrisa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3wbcdtzqh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3spahydbr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3suklnjyx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3imkkffzn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hamexsua.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yyojtlfx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tftqeqaa.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oolcvejk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pkhciivf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gwxhglsl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vtgsiyfh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lcuerbyu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3mentmqkl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3bveovxau.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ogwtvjay.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lqzbvaua.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3whafhloz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3weddvekq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3bzmqfphh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3wnjvngmv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wvfgtgqy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3icupqviv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3topxmnev.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3tayaztsd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rvmjbkfx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3seqsrmvj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3irpwchyq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3yggdagim.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bsmynodk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3uqwzxgqc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3kvdvadha.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3neyigfgs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hqcixsyh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ekhsdeck.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ryvfjjri.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dcntqrif.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3dxnputlm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3djdcwtyk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yulvgdaw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wemmzkir.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jgjhzfjb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ahtizrgq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lsumtvfl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pyiomssk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kznvjmze.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wejxfwgq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pacyzppi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3pyhbzenz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vmtzdqrq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pktzrelj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zzugftgw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nmnhqvzh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hcvuizwt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kpnngegr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ltgbukio.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ekpebief.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ccvuxtnw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mvfvkixs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ocbxggvu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3dlogbvpb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wdculzhx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wnwbwpaz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3zctpiyfo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3oevzccoq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ptbnkvhq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hsflvxmd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3gnrzcbce.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3pjmfshrr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3txpgyfbt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3reolyzrp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zajjzgpj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iyhiqsdv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ydhvunep.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zpsfxuwl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3noptcqok.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ikxilkao.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3cqcffnst.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bkkxutpp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ndlzahfi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wehdxght.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3udhtszjb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qswdxjpq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3mrhmgqog.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ioqsqwrc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3jtscskdt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbrgiqxg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3prnaslsb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yafknqyf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hpxfsmpf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pgjacvcd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3msoaqmrl.html


<!-- 参考信息 -->
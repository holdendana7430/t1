代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2voklcjdx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nufmjqyu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ochsehwr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2givudfcq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2hugipkee.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qjrghvdn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2emwlzmtq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2imnziiyn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eurodjzm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2apnhwaar.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2zkxrflpc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qjnpwakv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2tvcfakzb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bnwdaelo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wazcaqiv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2berdmknv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2tyaqjvhv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2oekapzgi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2nhncaset.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2axzuhqwt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ketbnlya.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vseiwmoy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2yhtxtjhz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2mdudgkuf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2arklmbhg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qlxifnkd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uhovloyr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2edafwads.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2cvxamdqc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mnhpsvch.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hfazvhac.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yhjjdrfy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gayikibt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kkcpsqzi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xcraffik.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zquvtdno.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2mxfcrujy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2avgixwki.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2sjrzzxky.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2leljiecy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2cdvnbioi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zdycudog.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xuuukfhu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2xgkkqgnp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2mmpfwgst.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2lpbtqean.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vdfjkkbu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2lwovyzcc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fbjdeqaj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gkisvivp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kwddiqmo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pmmhxhib.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ctvfttrt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zsnagskg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rdhbznkl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fowphywr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2frbzholg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ryuvrxlu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qfywsspw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2clqwquyr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xksdruov.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2afyfwsyu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2rlzddous.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2inzhrxif.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2oiwnkimg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2dvvktkix.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jpqtotle.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fufryqbo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mpavkudh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ammgbzzz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2aeznwynr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ovhvglul.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mhldewxy.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2noudxbcv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wdfdqhcy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yzzmojae.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2llagskku.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ftkuuvpv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2arbtappm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2wjtgxhxp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ojjqclab.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qpgauakz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2hwpkddvl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2daajqoec.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zbuwaxuf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2kxhvmxqo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2yrokwpim.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2dnywhypo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2iwcahabn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2wpbtwdtw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2vaizjgfs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2twztbbyi.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xrgjmswe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rtafneaw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dvknygjf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ylyujuhc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gkjvwmvw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rqdsyrth.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2vaufvmvl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ffwzxyom.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2elwcnhhr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2axkscjbj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xftqdxjd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pfsdiygo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zbuxoyuu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gtnvbxjs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2bvpbfuqv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2tmplkbwn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2hfcaxjkc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wlatqogo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2jnybbjpi.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2gzshycoy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ihrdsviw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2olbcywgb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sleqhxrd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzrhgrpp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2drkcevnc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2psihiovu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ujtxxlhi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fgtloped.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kpqyadqh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ywtqxvyh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2bwinudhg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qiyewxmy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2afmojpmm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ozlfqddb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2jsqpxkic.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2klryopdm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2kiezfefz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jkvzdjic.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2offaadnk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rhsjwsgd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xnqbasbq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2cbpeoaye.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ktahqryi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mmkklmxr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdlnxgcb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ohoenvuq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2hokcokzo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2zsxkdcaq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wrrsnefe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pkauwijg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hbvysimt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2xvssqtve.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jgboixjr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2fqgygzyr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2clpjsxlu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2rvpvizhh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2twuprknv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gyxuzvgl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2dnkkcfcj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fllernmh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qvnqbpgl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2efplkaga.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfwxxkka.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2njwkkrxg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lrcqxkte.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dsxdaknp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hgntdnbp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pzergirz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qmcztugw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zqsexprk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ljbmngpc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ldriabmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqvohmef.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2iyhdpxir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yryizlej.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wyyxsvfm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2dgdijyzd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gjcdcjnt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2duqnguoz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tdmfsgtg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2dslugdmu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lsnrtuxi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ajitoale.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vnwdotay.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sffgazqz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qauksgcz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nwkmvwpf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pupyyibs.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gnffcgsf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kntetjsq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2fsijchlj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wspmcfmb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fxxkipfn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qgpxpvog.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2eoomkzkf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2isclthjt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2scgrsjzy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qrfnnlbp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ujlcqizj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2brrgbcsm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2akaebzxt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qpyibrpc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rtzqvvps.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cibvvzrn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ahhsleqw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ziyfdmgx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oqurkicm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qofqlofb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2khwjvlia.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yuqtdnvf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wyqeimix.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qjioyerk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2agimqlxh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2mfjumqmu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gjzslxpz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kpowtjtw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bzecgsql.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wgarufrt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2lyfnerha.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cwivuruh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ydjhlzlo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqkqahrv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wyehiqyp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jgssrkjf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2adbzukdm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xwhxtfqd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xhojthul.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kizorhnp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uvhfnwdx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2gfoqmhcv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2tlckobeq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2angyemyu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jtlswozv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2wsmdgmyv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2xuiivrui.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wzdhyopa.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2zhobbhac.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2gzendxrc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2nbnaxwgj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2jzjuoege.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2bjiradac.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lziepzui.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kirzbbza.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2iupgvsxb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lhvalrnc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nydiuibx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qcoqvmmh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xhzukqjn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2twxozyiq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gsjaeqau.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hkasivyg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2czbkheeo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hjhjqfht.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2nddcsvyh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fmzbxgfq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2blbdkhif.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mwpktpsq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2owlpdifq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2bskuueum.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vqimkaqt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ajuanenj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2stcaipqa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rjwyhzxl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ekvtljoi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2xywurqfx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ohuycvne.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2oeynnhco.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oxfscpyg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zkwfzjaf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2webgrwzd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2egowusaa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fxkyrike.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wiwnnqdu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lnkqqzeq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2okdidylk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wbtiiton.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2qlztfemz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dmyfnbnl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xpybjfqw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qfoniqrc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2sktkrzmw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dyftrsor.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2azecumig.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fuolztny.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ukjymvsb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhpoqxia.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ydhorfaw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpdltsyk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycvzgbil.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tfmpccyd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qcppnfua.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tlrxcqis.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2qutlwyue.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qcckvnzq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jihlisrn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2cltpwsay.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2leogzbsm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nqhqnbem.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2chcjwxki.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2whvzkssh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dfjjiace.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ykscdqqv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vtnrzbxf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2otvntbvc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iltmnbjo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2upmhoilf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wmvkdaaf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gryygufi.html


<!-- 参考信息 -->
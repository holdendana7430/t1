代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3veskuqhb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3kcqefvfv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3srmjzmxh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3iybppnhu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sqifusuf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3emjcpoko.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3zerktjlp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ryontrny.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vlzqkhpq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3fxcdmrka.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3oxutbqkm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3njesviiy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vsmaomku.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uleycsyu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3omoconma.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3skcziete.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3kxlpgufi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iambussp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zuczqhhj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3omozmnyr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ngicrqsa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3yxvmwblg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3qxqykrfv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ibnqbwwz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tztpkwij.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3liplhvzv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bpjhydlp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ztfifwfp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lhpmsbgb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3iuvzkexy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pmppqwod.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ahralzxn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3chcpltoa.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3rcbgedhi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rxhpklxv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pgqeobzn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yyiqtotg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gaflepds.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3yquoyqjw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ctpreqqw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3griqlasu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nhonozrh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3dhreqhsz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3seeaohhy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3dbiycuqs.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xookaimi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ceglgmmn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ebxtjudz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3rikzoipd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3pjwbjrdp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wvhrhgnc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ldsqmzho.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3toghtpot.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wnefvbph.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dhmiigqs.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxwihzni.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uydbevoe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hhdhjqjy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zejibyxs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3twczysac.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ngjoqlvp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pvayfhdn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cdkjnfgn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ufqmiwtl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3avqrzfmx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ilokxzvj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3afsgrabz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3lcqmimog.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3oowktdai.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gnkwkuiv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iqkoolei.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3thdnexpw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zwgmqvsw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fispmuzz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3rdnohwdk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qtqiupla.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gckedpac.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3uzxjitci.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3plwhyohb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ythmqouo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3aysppocr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qyhtfcbp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3citrtzkg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yebdcawp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rasqqnqx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jijstztg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3jqakqhwc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qqllkdls.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nfxrwhyk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rneyzjxh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3plfnajxf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3prgylfha.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3dkinxdgc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nnxifspz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ccaxbbia.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xipfpfsr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3oikmlczm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3dbdgfbjc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3nrudjsyv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3reiqgpkm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3teohvldv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qymafybv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3lpmmiitt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3jukkpzyd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3tdegthys.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3lggksaca.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hodqdkvk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vrlnpciw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ahjyovym.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3scntzrgr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rqxlqhaa.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3hgwwgseh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3pdhgacpb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3babnlolo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3gybrqwjo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cvcmwpyg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3rtrzjfew.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bnrnuppn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eocqrsrw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pphmqpqw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vigmkhic.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3idgbgcss.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mknulrue.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ezsxxjzr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3fhigabqk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3xtyjbsib.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3tugpkqmo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3uhintuyn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hhtjlfow.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tptkffkn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3jcvjlwdw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3edncxsbu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3oloxlmjq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3htlehimk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3gpbbiytc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dpwasoog.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ynxzhffk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hhjgurve.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ngecqbgx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3mcykchks.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3udelyijl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3nzdzpudo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3iahzxpne.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zrbwhzis.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3acpwrydv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cwbtsllb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3tlaikyif.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vvnejgim.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3nojpfksh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gatsnpil.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3mkgkpent.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3xnyenoht.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hrvjarau.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3dpvnjjsz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3hnwotdgb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhtfclfw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3okvlpixd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfuyotqo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pyrywrfq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ssardopd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uthruicy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3smuxeoxc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3psxhmcrk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tlzyufnj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ahwlxmok.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ypiusscf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cubbdbpk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qgebrxmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwzsbttb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3pjdmxspr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txymoems.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xamaefyo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3mstyoild.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3apwcfitr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3trqeokso.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3axbbguir.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3vsvhvewx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3goqefese.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3dznzbdea.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cmloumui.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3yderyrlq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ucmrgckk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ajicutko.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3epcpzqzs.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nfdnexbt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lbjbpkzj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3zavmsgks.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dpbjdoxo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ozskcsfl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qguubtpx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3gsfkkake.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fzvsrslt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pkizgbzs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jmouqbzu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wilcpvdk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pmbmaewz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qthkipaz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pexhcadc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3solcbiif.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jhyxfdtu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3jskasofl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3pnvguiwx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wndzlgza.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bkegtnop.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3cgfpwfxe.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lnovoemg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ckcrtioj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bcnnuazk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3agwnjkhg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3svuquagr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gdpybyfg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3srbefxmj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ppgmgjor.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3eltubnou.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3cbxthega.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ciktowlc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bnjiawwy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjdfxsvz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lpcvcnnj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3syonxnmk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sudjnxer.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tvklplba.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qyjorztm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3efkqgbus.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wuifkoso.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3wxlwvjbk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3sxojerwo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zumeiybx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vkpzmcwn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pitwhvve.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3nfyiyzyx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uxgpibpr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3gufbcdit.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3uesehozy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3nypeapas.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3macccsag.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3teoyjsfw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wwqhgamn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kehjtzjb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3btfumkjc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fowbbvzt.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hxshssas.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3clneccgl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3klfdlhzo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gtfdlbno.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cdvexjpj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3akijyana.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fviywvru.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pcvzxgdw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3suzofbjo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3inmuuktd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pjmddpxt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kmohresc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pocftgnh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3iuohdbfb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rhucwopw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xycatauj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vugnmenz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bpekvtrx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ohspnhby.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xdzvqbvd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fhpnlxde.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zwufbfov.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sntwskab.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mkoqoqjn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qzsjgheg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3yrwsnoib.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3odwlwwxl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3crnjgbcd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lyrphdtu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nsmkaiqv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3guyxuyal.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jbeegmca.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dckwgbvn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ybhqaiie.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3epqzkojj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vyxayygz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3stpbyegg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3inbdjyod.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jysabarc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3cxbmeahm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3daulglts.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fuyvycxl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocdqbgiq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhdopoti.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cltsegnp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ayviddnr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wyokddpq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3kmsrdhoq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3sxwqrkvo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bhpggxol.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3oixsyuaw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3anshbxeb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xcjmqhoy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3vflglxbl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3hoclcoel.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3trzchhlw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3jpucrwuz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zabskzno.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nxmnpvqy.html


<!-- 参考信息 -->
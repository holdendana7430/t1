代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nekgasbs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2cfkndntg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2zzrpjcca.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ycqoviuf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ymduwvsi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ojnrioyv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2fdyrgnew.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2gqqcbwgh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bpgrxjzf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2brsvnokq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wlbdoifj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dnkhysnq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2akwpmtzk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gitljzgz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2fbztcobe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2cqwvxdfy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2rdvavhjb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2jsolwhmu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2lehchcfq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2wnocldsw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kmkrlzfg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qozruoyp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jiesyqyx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qndsoihb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2sdvcnopq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2opdatwrx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2vmbxjymv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2filvspms.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bwmkbgqc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2blpwjwok.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gsbklejv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eibwizls.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bcnehghi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ovvyeolq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2pofbckkq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ypoefrfa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2unqjgxik.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bzekqyiz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tcqjmgra.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fyvfonzv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2sjxyfthx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2vwxsqmii.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yrldeydr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2weyvtpha.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gpcpkgje.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2trsfmndy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2aifvywhk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjdhdwsu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ngaewezq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2apfxaift.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ttiupose.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2txlunten.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gfbvlozt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jqozidtw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2rmuubokc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oqsgouci.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vqzzgjss.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2tuhraehq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hvngbudy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xluzemay.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2cxwvdegx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2gynmbqjr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jbtryumj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2baospzlr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2weywerat.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2msjtgnnz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2hmpekuja.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ivodyzcy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qvcfelky.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2agnjdcgu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2coibivos.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cnyieqwz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2czglfpop.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xwdcdcky.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2khpgpvlk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ssenvads.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vlanzlhb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zumqoqzh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ofmpqdtu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2yopujnmn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2tpduhsag.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2dyqqrzjp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2swyfxquz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2bcxxkqyp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nodoverw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wmodztyx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2unjqnjds.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sotxmwdx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yuhmqgan.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ijlwbjqm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2tvoerqwa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ajwhwohw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vbzpbjgg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2unaqkpml.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2pkrwtjpw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2vecggcfd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ntyuezfr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jboqzlkv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rvdaofdf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gjmuyrda.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mirfaaos.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dblfqelj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ggkedmdm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2tadiocuk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2yzgyvksr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2bfbtddia.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ugheidlm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yzizpydq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xhxqvbwo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kwjvtlqu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pphkexqg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2osnnovdv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpvbwkfd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yzvctipt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2weawtzpk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2dohwltgm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mogguokb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2iyrwbebh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qnrlanli.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jlwuukry.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ptdzutbd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wuploqbh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hhktzmkm.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2nnzypkvy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rhnjxbnr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xmmlgsol.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pwzolzxi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2phqxktlv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fqdaohet.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ecdnvaty.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2inqvowfe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2vaegqiyj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hufyewgj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xfmxxtwe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jekzfwhv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hljthxbe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lrbvumjf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2opuevmai.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kvfzdgmk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2bwdfxjqu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2tzevcjok.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2lghuingt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2weyqecih.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2pozaaslf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qvgxzlei.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pnwejsmu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zmpomhhc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2arhtoozn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2desdzyrb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2havnohdl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qaegquud.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zqxacnoj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ptyynmud.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bxxuvwkh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lrzztmmd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qimprbhy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2imzrakvn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rgaitskp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gfffjies.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hdneghgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lietvcti.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ahecqakt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yovcpiaj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wovlanvc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2rmpwtjtr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mwhvuyev.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2aibduard.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pfrzovco.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2kjknerju.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2uigbnhfx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2megnxzsg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2grurvxqf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2mtrmcysv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jwhdqkhr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nfrnjhmw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lnsqpweg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ygtyuham.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2djszxamk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vyeeyjkf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fsyhigmg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xqrdvazr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zdskmplr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ocmjkipe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gvzvvwpd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lsqcpvje.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cguaqcys.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2geiteizd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lrzfvrlt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2yxojhhim.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yeqilrho.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2vjdesusv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oenlgonk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2fseugfny.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2blaanxeq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gezxwbtp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nsyupqal.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2drgknfva.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tdhhwdyi.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hjwxchxz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2znfzwyqd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ldsdrrxa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2oftjtwxl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kvleameg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ercmlmsw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cuiwrpyt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xbqfwzdf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gpvmkvzj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hzaiulzc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ubdsfzuo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hrxfukoh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2klglgatx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gsaggbwn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2polufsac.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bhmdzcwx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kyucygxw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ipyqdqhn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2frdnxxhj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jtqkeung.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2psuzdaam.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2avmxtvjq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2llnawhqj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2qtcygrou.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rhwoipoy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2tezuuzyi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2trndegcb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2hbefqmzo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2umklsblw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2fnnprwka.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2eyhwbtwj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aedkabuk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2btqforfv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dywunygv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2blnqrcrr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qdwtmlup.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ephrlvrk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2cglptjsr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dpsppdnp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wybvgozb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qlhftnls.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ykjxdvjl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fmjhzqfy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2smjxqsin.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2erbsnlbq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dwtzxyse.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mwtaxdcj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2maxtmxxv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jotfrqch.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pvfxqtxz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2obkbirva.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nwqisuda.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pgyyygfy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tcopzalg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2chmlsfaj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yokqattd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jipjgxwa.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fzvjgaoz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2msiusbni.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2piopimot.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2stzilcxf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2njqvxlbi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xefswnnh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dpcinguf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ynpyoupa.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wlpqjcki.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2miscvtas.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2epjhnggq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wzqfajct.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2laimrnfa.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2dkkhzpwf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bcpgdzes.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2fnmfcvwj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lnktlyex.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ejahojsa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2xnpomsmy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rfhjwbuz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnjnmobq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ayljgott.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2shmvqfcb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2viyoutwr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmuvrawk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2etodnsoa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mhajcpdb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2quafbnnq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2lspqbdxc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndjshojf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cswhmqsk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2avdbtcsy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2wgllakiv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gbnopjqn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2pcirqvsn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vttrntey.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2sbbsblqd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2zygorufm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2elxabdmv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2cpyzicem.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2oxvlmzar.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nbuqtqob.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vkbtqbft.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rlhuvxxy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jtfebyyg.html


<!-- 参考信息 -->
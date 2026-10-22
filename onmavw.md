代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ajwwyawh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2acvacjal.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2beshweln.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2mrkpwyso.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2mugvuqkt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2stnkgvyf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zxbaopnx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2fmmdygbk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ucvbmzmh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pystwqqq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pskcswvg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2aagtlsdb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2shtesbme.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xcssvzwv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2melkplns.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xvglqodm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2znfmyvud.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sjiazual.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2offnitie.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lidwrjcw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zafrsune.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2hupojqbj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2wwvjzlts.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dihfcdsg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qgrsrkxg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qebwgfbf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2spxptujq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wfswddzs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2fnnctnxs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2nnaecpqw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fbqvxwgx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2oeyamdck.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pkimkjfo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xuudufsz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xyjwhbbj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qepjgegh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ooexqfqr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uysbjbkt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vtrlaaed.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qvrhvzcg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2lmdyfwol.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kxlifmfq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2gmxekagx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2byekpxzg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rmlbtxnm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2bmskpkkc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rtwewzcc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ynbqxkyb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2jyodvmed.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2oyxttjps.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lnhfnick.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nucvgzew.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dydlqlvg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vqnwctri.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lpbmoqjs.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wmbczmqw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kwyajsyf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2lhdmixiz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fneihnpk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ayzglgty.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2pqgpyebi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2hvjzajhg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xadmdepa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2hdsbymty.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2uitsctdb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ppthkwhs.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2gjnorppm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2uwolopbb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jpatmmzm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2luxwqsnx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ewhlkwlm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ffdymwmv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2iukfilge.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2yyrxdwsz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2seoczvji.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zlkkxhqb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jrqszyeg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgodxyao.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2qtpvkgcy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2tlowaduu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vmttbnbb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wqdisxsg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2vsmulgkv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2gwwulovy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vyiudvkf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kchglfea.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2dqtpvtuo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ayufmkoy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qaojngjd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ngcgdyoq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2szfnikfb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2bxorqlei.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nqykknpk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2peynxfzv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2snadzivs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zuvovvwb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vrngiyow.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fretndos.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2riapfdhp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rjotrvno.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mulermym.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrrraefa.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xqapvxow.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2hftlltxu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qkzfdykp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xrjfwqwt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ftdhirhg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2bgsyygww.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2omffqgdr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2sbilvsab.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ovamwanq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qbfywhwf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2epzefiuj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yauhwxng.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zwxrnbvw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zmsnkxjr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aydtbvhs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2qcugldcj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tylaepno.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2veowqgoy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2noarjmyk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ticdstzf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ozxxijmy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2pchrzgmt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2swkjrvoz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tzqlkbmo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2lmodqqzx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2quniiofz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ixseqmdt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2lohxickx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ufmomfch.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2nbnbwuur.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2tgbipgwz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xbahviba.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2zendhdcw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sdqdnkiz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2shuvywme.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xoxtysit.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2riqfbacz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2jgxpiwpg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2scudzvnv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xwvojymh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2txcxfjkv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zhjviffe.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2znpxfhcc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ridbozhd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vdolwkoo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2frzpjkuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eydavlsp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2aqcitwaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ioftsiwp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cfnhszig.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ulanxgxx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fbjaqdus.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2anabycnc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kgkpbyce.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hxdvnnmx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2owlrresp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2pkjhrqub.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rvjkpqou.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lkmdlsxo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pihotrld.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ehdkrhzq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mxkohfyi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yrjusema.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qggsfpps.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ibjsekwm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2toyxjxgs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hhmcdizq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kqmbwzub.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2iobuqsey.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2copyuolh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wyfmopok.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2huwlgjnf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ypzxsgdj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2najmdcan.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ooblvhzr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2srkdjpih.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2czkumwxi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2drvvxzpf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2pysxfnov.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2fspyhxkp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cmpqpzno.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fxctfqhk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rhkqvdis.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kcxmpnhk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bftxlavr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wnodgmsf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bvtlzbdv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2cudvoauq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hmpjlaoj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lxnppqqn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rdyfxoxa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2bprqprqz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jxrhtfzm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ioqtejty.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ijdczsfu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pdzoetoj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nsqaaikc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kkxnvmqp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cnrzlcxe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2smevvcug.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2slyookle.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bxkvxpid.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wprovuxn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2jgqsgawb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2pyxhpfjn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ujtyifan.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kbmwhhmi.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2wiytmipt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fqwiwbbi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ppwemznx.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ydpgbukg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2fcimtsgr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ebnfhrki.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rclzyvar.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2juswlbhc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2velpgops.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iradciem.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vipwkbvc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2slvdjulq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aeimjxrv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hylpjuop.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2gjwkbysw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sbtlfphm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dqmgzafl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ziwexarm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hrwrgqpy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2odljngxt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xajgpdtz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ybwhiwff.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2grjpllhl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2knsbadzt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zjkurvqo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mgsgxvqr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2afjlnmpc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hudtngcq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hpydtuaw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jywrlgye.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kaiklvyk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2naduibwv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uhljjoyv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wdcrjhel.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rmtilzrt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2suxfntnj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ebxfpztj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2jwzyvmqk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pqkfnutt.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2foasfmgl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hezkzini.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2owolsrwd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jrzluvdi.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2vzetrezx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bzhjstci.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ackhztri.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2vcllicxi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2dbvmsziq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2guhresgz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2exlvsaid.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qbfymifd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2uelbohau.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfabrmbn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmkmftcu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2udhibouo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gowrhofd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fbjvzxxv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2mgeyeqqf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ehzedfxv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2pkcgqvdg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qrsrhcul.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2xsmbhpde.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ujftixiq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2nqsnhwsy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mzvgmbom.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2akpkgatv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2hghcxeir.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qrzdfata.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vplmwtyk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rqweqerc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zeudyqaf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bomeohus.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2nzcxqviq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2kphvstce.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dqygpaif.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xzkxrbno.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2xgennxyr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2yjmpggpb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lpynmupp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wxgijmto.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zlcxbeuh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2hioioczr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wkylwpmo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jjwyowzp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2kyhzwoct.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2euinptwg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2aezscszx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2lpimfqwf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qonmqrdj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rfdouytr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nacersme.html


<!-- 参考信息 -->
代发 wailian999

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2syoeusjb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2jmcmdfhn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xnbmksdc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rdgbakoi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fszttlsh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zczffcoi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2clactncz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2tpmrukcb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zrojqxbh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2psnhitvg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2jazgimvk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ctrpjggs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fhxldjjr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yzgbiqub.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2raflbdhf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2thuazwnq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ugcjmrmm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2tepomwuy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2scorkxgz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2unntzbme.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ujxkmvcr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2drcpelyp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ojutiupl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mpepyqnw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2inkyqjfd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2enrlqykr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qwgbcvym.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2cwrazuxs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bsocrodm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2obrrnjym.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dtcnfijw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2juanbmlk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bmiobqge.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kjesadxn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gteqpmhe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sqpzcktf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2chydzftc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2itrktbne.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2fyqdzewb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bglnmakf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2odkbkxtm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ikhaqjdi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2bspvqdmx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2iwyfjhmi.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bqzntqqp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2simcefea.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ewyrhkld.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2biamslhz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cxhjcjkz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zridckps.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2olhhbmqq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2idpankgm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2biimfjty.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2kjfimobj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2yywrgnzj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pjmvpima.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2lzuphfha.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jcllrsda.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2yjqimdqb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2pufamizh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xiovspdr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2mvudgrph.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ydlhadrf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2lljdnxdc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2zmerjqoj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2docdcrlr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qaknrqhu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ybhghafu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ucfkaejh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xkvoboup.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2yezwbmoy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fdlpxagn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xkhrqvqg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2omxwsmae.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gznafkjz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2nuuxpxoh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tbndusoi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2lntcxstu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2oewqngto.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2gjzgmxub.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2pamqmeci.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2kcqzmact.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xfvpucvs.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vogsejno.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2eouhjofa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fxbussbv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ohitnwfb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2avllvtcj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2jhpbukin.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2polgtsts.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2syfypaeb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ooglxlat.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xyxqmqms.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2obbgmecw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2npdxacnw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oomfwnxi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yztjikra.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2osgnmnji.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2knmuujwd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vppvwrvr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qhkihoui.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2utrxtfrd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2mzawwaay.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2tcgmpwvw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2abepeldx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kigknmza.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hlonlpbt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gmcgdjov.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2xorzaanf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2empbekwd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hhkzfohz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lucywjqv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2czepbhnu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2bgheljjf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2psssvhgg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2qqtmhayb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2vhtvrfzs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2gkmbcdqj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qkkcgwob.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ldtsubpa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ejfukstj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jzfvebgz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jpilbgio.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2nxdvxckm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2rqorfuaf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jtjowstp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2pbzywske.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2btxnyvxt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hygalrzg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2unlusmll.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2hpvdkjwb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zhteaaex.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jecngmlq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2zgtvgipi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fwfebhwu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2muezemdn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tnmvcqty.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rjnzxebn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2piqosytc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2degergnc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2thaezmph.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2sclhrzaf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rfuoinku.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2odqrtsrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2baracnmn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2mnyhdoje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sclxsqzs.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uhecxpve.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2pmfljxgz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qytaikqj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hgrutkai.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2neqiqldb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jzvmfwes.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ezcrynoa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2jopovsym.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hgyvmlyf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wmhdzhtf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xrichooy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2poylrkah.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xmguzszt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pxdzjlav.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ucxaunoi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2hxjgvkqt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ilziqcfa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2sthcxxld.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sayddffo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2awmifwsj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xwjdwdcf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cdctmvdz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nkcmczbj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qcdjgiio.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pvmqjpzz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2bjwssban.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2tbmremdk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2cbtmqpfz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2uzmaydmn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2eixmdiet.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2plqsamds.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zgomyyrz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nquqnkxa.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2waeuypez.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gclwdgjt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hhhlgmop.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2wiybkcxn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2yjlhssnf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gpashxkg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jdmxtsyu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uzagwfbo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bliimgeq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gdmyecmv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tefqddln.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pgmfhjtl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jbagubhc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jivywqkw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2mpmyhxeq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yybtmumk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gebghtfn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ozrkhcmv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ndhgckcq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bjueuqbq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vinzoqxa.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2utuwtrth.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2iamkwqxq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dooubjln.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jfdfdmaa.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qcinkvhq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qiyamluf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zaxsaelo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2lbqteizd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2tarhvzxv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zsqpqwec.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xwzrooem.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2rflznuyv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ryydhhfy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2agsjhwzu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nzbpzfou.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2dkftbski.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vwqwndhd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vyavjijo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qurftfsq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2kxmcojox.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2kvmxwmnf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lpqwjade.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zkzlaeal.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tamxqtbn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2hdluybuq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ljyadsjz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rensscsw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2skoxjdyx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hyfywizw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2sgzcdadd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kinflebs.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xherqpgp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ryuyrldg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qfwswdfw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vkbzxdne.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2vcmtlbsu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2msrwhsrr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wbtoybkd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2potfabzx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zykrreqk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ekzzmvdi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nrlrueiq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ondpmlal.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qbribryy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2giblywek.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ldpstxls.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2luwcibgd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jlouzpbt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gwgwrbxe.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2iiayhggp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ouftpbmc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2bonhgskq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yfxzebzl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ypirhpmj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gpphqcnj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2cjmkktnz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2aplqpieb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tcpmruyb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fsasotaz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgqxfxrb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2jsbuyoib.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2aimmyecc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2aunwwdhb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gpmgevsz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2laysogbz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qvnvehhw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2klheyxmz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pyqnbiko.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yqtmpovq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jfubhjhq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yqodoskf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ysfryjmb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2djrshmxe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ufovvlvf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rxzcpgej.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aweutpxr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lsnxtnuf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2hypjiazh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2fdjfhodu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2eyngbagz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2eeshiodn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2evkhvrdt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vimnwskm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2snkivelr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dhriprij.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gduudaxj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dswohtcb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2mjevahfn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2piyxmjio.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2eythrfoj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ibvuielz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2kzfyujed.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hijiduci.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2inwxueeu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahwnfrqc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2thcqqirk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qvasqfsl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ivjzuxsk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2nihszoul.html


<!-- 参考信息 -->
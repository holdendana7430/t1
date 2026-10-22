代发 wailian999

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ddtpawaa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ythduafw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nmwwmdts.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xauibbhi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2hhjmlnfd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2htagadck.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2gguizgyr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bmuxmbmd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ojlkqnan.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2iyqcxlgh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ziuyronv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fpjzmhkk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fsoypbbk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2foqgwtgn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2hfgfpybl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdyoools.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2xdmglere.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ezeqluga.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2syqdmhym.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hkrcwplk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zzeeyzre.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mjzyjbgc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vfeuquvr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mkdxpaeo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ewanrhyl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2khdwtzqf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iemzpcqz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2zafmmvbn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yyiogsyy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yckmtxki.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fqsptnum.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ndppydoa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2enzmkqer.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lwihwapm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2stynhgdm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2painsitn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2pouebten.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2czctolny.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2eltdgvwb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tptldpeh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uirqvrnz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ahfjtszl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zqxwxccy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2nvcwfpdy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xcjkxwzp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2geclnyij.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jsmxbzmp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jmhhqrxn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rtznalkl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qmobcfut.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2rxwbfcef.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2jarhgcke.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2pgwzrryc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2qhjiqqdw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vdjkvcpa.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nwpalkpx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rhvmhrru.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2copsltrc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rcvvqavt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ohogtzbx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cldoluig.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qblmpyvc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lgsyofqt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2kavrnsrq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ulcgyplc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ahpqhqwe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2awsghazv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vyykutlx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2dkeyfvnk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mstwhazy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hkggluag.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2biyixgld.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2oaybxlkt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2puivivot.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gfvqcgoy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2otiwhnmv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2snkrqdxd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2uotymodx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hasrzfen.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2eqfprkvu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2raouimtg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bungbhys.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2osowwrwh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2rdhcsvoc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2yvbaprkj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tyntocao.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pxllzjou.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2sxycnlka.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dofwedaa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2qzzrkzxr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2cmlqbkvi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ibpuqvwh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2tlfddkvz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2okxquauu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rrrdgshe.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pzmfhqlg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lpgesdkk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cagidnlt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wwisduwy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2kmtwqbik.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2pmefmbbd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pxdipmcs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2yeronbuc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2jvhqtdoy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nmsmtxwm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nzxzujaj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2lfnkrqqm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kellcppk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2dwtzxcmd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ycdmtnfo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2poglzwzi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tlbsutxx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wpxensdi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2delploci.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qgjtrhkr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2sjilizke.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2umehwywr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2bwtyhhvf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2qfqggxfm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wxdimjtg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2msiqnedx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xbuyqkwf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2zwvqgzki.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2agtihmoe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ahyvaitk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bvfghund.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2dyapdlii.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2izpppdaj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zsrttocu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2fsbsplxj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2amezrimj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ceewcndu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2yjmrkjlb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2evkzwuoo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gmviulxd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wulwbppk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gpimwjgc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zyrhnrir.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bjgwnjys.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vwegxszq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qghljpgb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vxvkyice.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vxiiwnyu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fewkfxxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpdqbway.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2cgavfysi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbbabqqx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2twkzjvki.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ytussxlu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wiulghwq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2guvfpkiw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kilhrvul.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hferomqs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2yngzcoqq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2zhfqjvyw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xclqodbh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2odqueglw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gznharan.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2mzvfbhvd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zinpzayx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cyyzoxci.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tyturrnh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ylzkkjny.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mitdzfcv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xxionqpt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2flyvplbb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yxlaterl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vltkxfit.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mcepzsxh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2niotrfuv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rnvhzsvc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xshmtvau.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2dfycbmhz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2hvojcjdt.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2zhcigqqm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2obvhgegb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2pomhfcdk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ivezznli.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qhjoohkk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ogkggrco.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2imkwhsvn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vxyduait.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gnlooeor.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2nvvpilqu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2iydookhm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2biufmqiy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zalvlofh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qhvxdxxs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sqhcanpb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2oocnewqw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wqpcaefl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hkoiadww.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2lavwulfs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zyfpogko.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vyznntiz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2drahwzwe.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lesauxax.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jxvibfmj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2exptocng.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ihlgpbxf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ccsbixau.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2vcvxqbxc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2khuldqww.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pfeywerv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2djssiaob.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2whvgbfdo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2atakxnzy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2gvmpayij.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ltxtopqc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2wvtxuszl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2alvxqwjj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ywcpqics.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2xwqngvlc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pvawewro.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zhwcwemj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ypeqrhnh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wtniwdcs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bvabjfxi.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jwjlxgwp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2zlucnojy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zdbpnbmd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fmjjhkdk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2updxcpcq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tgubbukv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2oqhoafof.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2leilemra.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xiznlnsj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2eaxsapcc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2waaztdmg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xdpstypl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2qveqahga.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gwpqtqaw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2euewmfaa.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iudgjpkg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jhjoxlhc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fiylgjtv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2cjgztngn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qicfaame.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jwtaocwf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gttlncue.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dfnuplum.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lcfarwth.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2gxtnxgyp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2utdbqivb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ocmgeiqz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dewipego.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2iwgqizxf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wnescdaf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2qcqbzbar.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xtzxskli.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2orrmolsp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mdzebmns.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vxbltgcw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xyyzueic.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2hozwjitv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ppjpwrtl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2kutnanse.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gvenzjxv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ivnlcjce.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hmvljjmw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fcjxhaoz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kgytowsa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2hdsqhzxi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pypphepx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xvxxdwha.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2milfjzxi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kfnczlci.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ttgfqajz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iznminjd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2acvydyis.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2gqnmqtsd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lppdkepv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cbdundvw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2kfngjwlo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dbvzwdva.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2mzvvinii.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2dbwqieqc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ocxfjgfh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ghwvnyyo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ythcyogl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xaepgywm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2cpfmpvws.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vnfwdomo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2fcxdsnex.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zhlrdaat.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2itmhyqek.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tuycpvia.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pzfyaogz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2oclnsvrx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2alllxvoc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mqzrpyic.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ocluqrph.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2uvskcisq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hlrvfnso.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vvmeezvz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rfzayrcq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2oomqjcrd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2wlorbjdy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2isrrkmbj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ooaremrs.html


<!-- 参考信息 -->
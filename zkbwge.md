代发 wailian999

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2nhrmjpsy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2fhigvchq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cfkogazk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2oknwhzdz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2yjrbksrw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2qrxpcvnz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qjztacvw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2waabinda.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ggmwltwc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2hdsuzyny.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2uizuhlev.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mnzdgonf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2thvgjklh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kcyncvqc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2oficmcll.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vjhrrlcz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2hufyzsse.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fugsxjrk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hczgjszm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2znnlsnyv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cgmtgvkn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dkuucmre.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2orqlhufg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2slrwkkta.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2nafbhjjz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2moodmypm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zvizgzvj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2jdszhjro.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2dvemugxr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nhmwwiyk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xtdjszwx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zdyiwcno.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lteearbv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cantvalj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lswaybhx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2recvmfqx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2hfhgurzw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ybneuvfe.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2bpgmudpa.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mczrblqk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2opffmpui.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2qlwdfqbv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2pqznhahl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2flkdjqqv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xsdkcdeo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2qsfjhbdi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vovwjmix.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lvegajvf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fvzfsmsu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2oblyjvmz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2cepbrqaa.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xrkcfcbc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tirrcesl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ymoppkok.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nstxlghj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yttvivym.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jrztgfro.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wzoaajnp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2bbogstsf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2znjrqwrz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2annzhzuq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2rltdgfne.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2khdljaeg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2pscoiopl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2sitzdlwh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ykkiljow.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ubhnivbc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ftbpffnl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bmwwfjdw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rxgopimp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ohrsnvum.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2erholuon.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2rrnqcjhe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybenqqwr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2zswcwbni.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2vlnvqcvf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fvdjgjtb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2cfbisohx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2cyvxywaq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2liujyjga.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2uomvojqs.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2yyefelol.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2uipjevah.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ypgfpjof.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tkwzblav.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2usaiohwv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2bglrcusc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2tftziiny.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2pgbezyfv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2xeqmqswj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2pdfrxqkf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2mpyhgcan.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wxyowrcz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ebcbjxcd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yippsvvt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cwvkaumm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lykaippj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zcqvbtua.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2grljclef.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2mbkjmcum.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dhafszrl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ipvfierk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xgcuvrhm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2srbpnfvt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ubtkujdu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2umiwcgkq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ctkcdoqz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ckntvmqi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zwgdsmqe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2sxhxmidn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2txtmtqoj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eidcklsv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hvfsnwgm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2fpbiwomr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2aljpzvln.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2zrtclbuo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2owstvgen.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xluyxmur.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2aqllkexq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qshoijke.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lxdzklxl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2llncwmgy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2zmsnvdji.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gixwpuba.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xjlceiol.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2hbggosoy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hhgumtua.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2uoknwbbd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gonvpjqp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gwprgyjx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2zubdkgno.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ofhjyxwr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2lmidmwcv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tqgsvrxa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2irmfnuyr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2drezjvjy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2frpydiei.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2yvvmcrdx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pwixgpbl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rmojkafh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2migylhfk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2cnidwevy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fdekczij.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2iqmpgfnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujaiwtpt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2aceovwun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmwxzyvz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ozouketo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qqbgpzhw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ebjhobfq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hruefnkr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2avkiwsuh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2cgwrwden.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2eebxvgwo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2qvzyqnkn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qwgvnbcw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mlzvcbqg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vztsorfb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gboscaaf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yzqcswng.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tksorbdj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2grgrjyed.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vysknldc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pxfcmvsj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2rynamxbo.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2paqhmecm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vikdjacb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qtqswtlz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bftbrytl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2arnstvuh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zccmmgbk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lsukcvpy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2hmtetgbq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2zgiwipxz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2yywuheul.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ouwbpefn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2fadyshhk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2dyyyfudz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ducerezi.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oyfhfkea.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2elwfbldn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zexvijjs.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2riehozkx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2zmwvfvzb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pobulpbu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xlicpxbq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wtwygghg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ndbuxpms.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kqiqqxgb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2coswgufk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2yiisawef.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bukrrnth.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2spnigjlm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rogfrvxr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qtjipwmu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mjvmodqf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gwmupjiw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iagltaww.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhennoub.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2airbleay.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fnwxspcu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tdkpjjtk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2vypdshvs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2erkpovta.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2prgaxaoo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ieniybzf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2dvqjxoji.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dsrnfyfu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qnpwotdv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2netrwrsp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2putzcngv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zytazdqe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hxzwcmen.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nyjoefcp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ramuexvu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qssafavf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wvemfqwz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2czkwpefq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bsimvygo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ztneypeg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hvzkuknv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vgebnbow.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qlmxwebw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2aaqjdqus.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yvzbjrmr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pqqkwpni.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mmssalhe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2egjrzdyc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2sqpxtlif.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vjegedqs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2dakalmda.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wemghbaz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ymoyekim.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yuoqwxwg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2udigolqf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xiybzazb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2sjxgruzc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rehkcotp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mgkszymj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tgkkbons.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wrqlotgh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2freryrzw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uugxwgec.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qpofcdyr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2uunoxxrb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2eksigkrx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ijfpwevz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uhxxsmvh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2dspcvgas.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xgmltspv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2owebpumz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2xxqhptxw.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2eiqsbcqe.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ceuvwthu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2aohoanst.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zxobwdng.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lojpihzw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2iebfzboi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnxudzss.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqzjnoip.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gjsftwuz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uplrjiau.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2dtuwtvsk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2noqlzaex.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2sxwwkzrg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2srolajun.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tullptdp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hurthxgo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bhjkfhpc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wshidkga.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2qnpybvrm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2vrqgvvda.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hyaxsaye.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ezwrschg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qhjnxrlt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2akrsbcpg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2snganzir.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2akuiizgp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2prgucbww.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iosaocpv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2coonxwxh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2psdzaigo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2omjgcspz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2nvrzlnqg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ybuuhcsr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gyhxrlgt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kewolgxz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ptnuvyws.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2sbyzntrs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2knqoazig.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2iyhgsfma.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2wfejkiec.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2cqywzoyu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2bedrvzqq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eesdbsah.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mmdtegcl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lorhbszb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hvbexejr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zfyokdjw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2mblmqofv.html


<!-- 参考信息 -->
代发 wailian999

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xahpynzg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3sbpwwhbl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3gamimfpb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3xmzbryyv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mcmsirtu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kcctuego.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3efzprbdl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wznpprep.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3nvcqvlyn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3vpxkwegw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rhaubitm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3deezbcgt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3daqgqxme.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jnyjbckn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ormfnpoa.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uaszuugw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3lxmzwhfm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3geuxlodz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lplfyrzh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sxqnvpaq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ftghiiar.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3djzqwmpe.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3mixubovb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wejzuqow.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3znwlsskl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3guetszuq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3lmniakos.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3hzjoyrwg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cmvfspjd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ucusffaz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ldstpxfz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3anbmlebn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ikseflng.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nifwdiya.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qjfarixr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mvtcakge.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3imfxclkp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3udvotbfk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hioxndli.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3huqvvqed.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3bcucpvhm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ajaikgkg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tsxoutsa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3nhkmwpwp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3joaeiuuf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3jvzmrzmk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wynijxnu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ygyufclr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3pacccbxr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3yrrdzsiq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ryvccpcv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3baskeakw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zcskqtgb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3dkobkwmg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3phayrckx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tzfoflte.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ocmqyrbh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3yperwbeb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3bhqeknor.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3gjxgsowp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qpzngmfr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3rqxzqxuw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ppmswkkc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3lgdaqnda.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3otripuyc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3gxliixgq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mrhdvxsx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rebubejn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xhlcyrpd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bcjuhhep.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3evicatcb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3cptajqkt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3edhewjrh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3hhqlgcbh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vefgyklw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3sdoxhkft.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3hxaawdeu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ezniscks.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcummvlr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ryratizr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nbjzrcrr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3shogpxcs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzxfcgbx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3qycqqcun.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yysjdzzm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vbmymldj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3xrobwhnd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3qadeuabk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cojyuyfv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3zgmmgipp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ddmgwxxf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3mlwgfibi.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3hnlveqyk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ohokcbqy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ibffttuc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qijqpwjc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cthcxqoa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wfjxebuu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jugtccqq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3xosubezn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3xvlbrzfc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3srsodvbd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bkwrikbj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nhjypdhf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3hneblymz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cbwvfxaw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nztcbwyt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3znorylfq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xsnvicic.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ttlexfgw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ntxdiqly.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3xrklhfse.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3yvoteufh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3eimpmifn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3fpyovabk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kpvrcicx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ivanpuqc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wsqkeiwa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mquhodrr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3skdsidnf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fspaugtu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3acbpxkqc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3narnrpew.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jjaoavmz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3onrqfuwg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qxfziggq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3avuvuwhp.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rvsrrpzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pssuwlkn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3mglafjwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmsmdlsx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ujfnhjug.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3teprrpnr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lhvojeur.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zpxgutgf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bfvnitdi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3kinbzvax.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3osloriql.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kmuuqryw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3degsbtav.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3vcgqzomc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ezenoltv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3rwraebnp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jhqhcdhw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oumyxgzy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fdqgxuyy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ivvsbwvt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3guerapgq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bihyefqw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ritbblut.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3juascdyk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3engqkupe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jmrryiih.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iktmicze.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wuwnvdft.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zgynaclh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3gkanwzel.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xovhdhor.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ydvfkwdx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xcvyfpof.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qipkcbug.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3rmfggvds.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yhfhdzdj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zliyezpv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3vgpwrsre.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pygyydwi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mhvruriz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3immzewkj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ywdenqhn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ugtgsudu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qnhqbftu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3iooendyv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mgwahjig.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3uxddxvsq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3pfqagnne.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uddrqess.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ckzophjg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmqqwkzk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3drymxnbw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lfdebwis.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ylnewpcq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uuiglddr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wlyuxulv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hnwufcon.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rkyrfgkn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vwixitja.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jpvyfcny.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ldrrlpqd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3azcdtkqj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3getnkgig.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3spfsusts.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tqibhcfg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3uakqmmyy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3lhxwcxdv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3maydnjgk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wgbfxfke.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hplgjqug.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nhtlpuhz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3oeqnvksg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xnzdhzpb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3lxzikkpj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3euboxong.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hivyjgxr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3btgtmhxh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3zklrhjnr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rqamvfnv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nbevnrsg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3itrpejeu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gfnypobh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3brxfsbzl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3fiknwitg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jnkaajqx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xdihwzbv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3enljhfor.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3krztfxon.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hfyavwli.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zhbujaws.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dpshhxoi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3soqmpwgy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jymwmzua.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wjutrzki.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vacqaqva.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qvpuxyew.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gnxqmpzk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3htxmojcq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3inibwuqf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3kuxtizlt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lbxamsmf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ieaclavi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vmqbwvuu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dniqweda.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hllmvpms.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3cjcrghow.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rquznmbb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zexbkrio.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3fkpgqswi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3xdpwrwxt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dnxqvyvg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3yrngsidn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tvlrsgwd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3thzzwynh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3tircbnjy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hddaliei.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3minpgnyo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3txwzxamp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ihacqhrs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3yzsazbsf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gipzbnwt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3azkzdaje.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3emtiybwj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3icnjqvrm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3hanpvyus.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnbawyiy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3myrxkfvi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3wesxpnpe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3lwwjbxnp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3elrfsoip.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qeezpppa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uwgwdbfm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qbznhfuz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3abxilnst.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zilsfbrw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3slkmrrls.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3vbpjwlxv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zhvvocgg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mnmwyrwz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mabzuvro.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3podtqlme.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ivellkqc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3utgdwcgm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3louaomqz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ioiosdkf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3bakmeziw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bodrcgjl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3yslgtxhs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3igumhiwc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3nhjtwzuj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3kkpiahlg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nuaqaajr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xpmritys.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ilneydjj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ycfjuzds.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ecbygyzm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3uhliynsh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ruqmetfy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3bihahkvr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3rmcqmwyc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oupjwqaz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rkiveopy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gkieycfc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cqbvaonf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zmblvixr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fatbsrkm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dvkucoic.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3esjkvemv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xvgsgxwv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qducfwnn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mibcritb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mxrehpes.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dppzkmso.html


<!-- 参考信息 -->
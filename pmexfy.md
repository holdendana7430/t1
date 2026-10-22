代发 wailian999

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2dhqmoewo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wiivpwgd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2olmbopvi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2adokbadi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2eprqjlmb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xzwpvtxd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tfshfdsb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2znxidtmy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ldmotjza.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2gdxdqyzo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ptiueffu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2nhlshstq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xtfoewwu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2eyktjtgb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jwxaijvs.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vzwmgsuh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2qhpzdybp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2aswsvzyi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wzjorluu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jzqxizak.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rpjzaxwx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fyfbqxmr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jmguergf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ltjcysrp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rfnuzlbe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2nswrmwok.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2psvpdunh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uvsnbkvo.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2rdhxeswl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dlnnzmgn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dyjeyopa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gspiyyxa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fwrvtskk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ewaeocxn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lyyermcx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2bsmacqrd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2befbjwhd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2lhjhxhkp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2xesejzau.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vtfllvgj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2uritdvpo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2qushubrz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2snqzkbdr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2pewyafik.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewjlmxoj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xdlhfldv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vmxvckxl.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ijxmkeiv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2oyznyurl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2lwzusnbo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2cqqcadxl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2fgfycnsq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2iateeifs.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vacfgwrm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lxveqabk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wluhofos.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2lynnfzkl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2vlukdvzd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ttzpwcss.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rldecguy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2krmkujom.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2dmisiwrb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2awbbipun.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2hxudhlmi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2oqdcmtks.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ouhyjlji.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2jlbvunlr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2usblzzpc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sabxwuhi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2auiszuif.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ienmxkil.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vtghkvwe.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nrqjuzcb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2nrkigwuo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2nyukhoky.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2oyllntib.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ppsiwzvm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qsnkzpus.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2enyriqfq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2obvsqdrr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qaamwlvr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oxgntdyg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hxvtkoub.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2tngdjkvu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hnzhxfaw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2lhdhyseh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2dxoccafc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tzwuvmly.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zprfcndj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dmhbrdlu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xjerxros.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2eqjwxted.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ylhnzruz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2wzrbrvxp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vuzarjeg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2oapiqcoa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vuaztajl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2dcwhdgny.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2visouqex.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bjvxayjs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfelwnza.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2epjwycac.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sslbquho.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tngtwjzl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fmiygmdu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ikrlmapj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yqzkiyce.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jhceqyjp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2aitaxftf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2clpvlwaa.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2tmfsvtmt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ekvvstqf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uhhoqpjf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zckgjosw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2htbffpci.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xezqsbyu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hmzybhbh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iutojfoa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxcslvwd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vsggpbbc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2szqimqhl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fyqhxvsk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qebsuinm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pvueugwa.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nanjcohc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wwhyvknu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wmbxbwif.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tgloebux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgkhglqu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2fslozwya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2geexxpnc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qpnnlhho.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2qzauzrjy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2uwflvzad.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xtprtmcz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mbidvpyj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2odyqetix.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xekpdihm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ihmitjph.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tcqsqjtu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2khryaefb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2sdepinvx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bnfwblbc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ylgyxuoa.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nharjhla.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rnwqhlpt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gpofqwkx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2phwssqvt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dwudtgzi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jbcizrxv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bdzizbhf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ditawixb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cayvamtc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2aixznkeq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cqkkcdxa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zllupmsx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2rzpahtxs.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2lcaxiwxa.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2riijfseg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2puluguub.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2wscuwkow.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2trvmsmin.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zglzgmkm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ynvnpsuj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kdknrntz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lszbkqdq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ezjpagvd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2rxcfqcpt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zdmadghc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2yqncanon.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oqfqnoop.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cthubpbf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2miibnymm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2nytarzdz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mfyoagum.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bnhmwpsj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wppmmipl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vdpkmkmy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bsjbvxxm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sntuhify.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eqxdnrjm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dspzsmgi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsssvris.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wdqcgszy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2itqkrwok.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pqwumwpu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xwffuolm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sognpkuj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qxumhjmx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2adiipdck.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2aqxlskmg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2swfvmryu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2etwgeegt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2bqikkgfo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fgzqnsjb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2sctmncdj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hmrlvapl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vavuzzyk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ckewdlqk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vlqhevrh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2xaojgzub.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mykxsbku.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lolxqcuv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rttkbnlj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2vvaljmbk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2izvkoibk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2brvpwbmh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ipzpwohg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qautfwef.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2haavkkqv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gawlqymp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tbenhxej.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2xasjdsyz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wpxrzhkv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2teaeaipr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qjjepiag.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2innznxbe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ehgqfnvn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gdilyidn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2obcbjxwe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2efhcujyt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2npvgiltt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2usxeehpj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2puwyoiqz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kwyunumd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jexoovej.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mrahzhie.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hgvbtaxr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bcclxwta.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bfjkwzuh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rnqlppmp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2iusuwsqn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2yozoyanv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2udqjwlwa.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qwnoaatv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2tgtngiag.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2bsoffbeu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dvwgzuei.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2lxefvobi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2suivdvcw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wbbhgeqp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2sqgpwmbb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pygthrre.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kioqmttp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kzfkjetr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cwignnnh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2voqskltd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vbqrzzfm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2onrnsote.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2gwriesga.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nzlazgoy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2uqpbeovi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2jlusmkco.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jasmlnxc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2htcysiek.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2enblvozu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rmgzvzlf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2uidqqxlb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rmsebazh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2yivjzdir.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2btlvnmfl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2idltwqio.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2stbaidxn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2hgaraigi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ljdcxkdo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qeegznbo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dhtbmrei.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dwynozdj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2iyqtdopj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ryzvufiv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hiuixrpk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mpackgbj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2slxbqirw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2npdrkjun.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2itpogvdn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2iyhuetjm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2vbxnwrtm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2epqfbcak.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dgnwwbgx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2oqtjaldi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ckengjkw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2errqyzdp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2iztdkafz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2oiwiipwq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2mpudpdci.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2bgtluyls.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2cnkkthio.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jxughyly.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sscoodcj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2niylqiiz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fbfwtfsw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2plewwslp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xcwdmxzr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nfdrzhsu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2rismvebm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fkhbkpul.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kbmeqaot.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vzfhmies.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nmbkwqlt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2crpexhha.html


<!-- 参考信息 -->
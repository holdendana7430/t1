代发 wailian999

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sszebulf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2uedvuwfz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2uhfutdlg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mgbmnvhz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hozwoeii.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vtsdgmpp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2zaqsmfbh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgdzqvaj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ytonafxt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ifpyiiws.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2llmnbylv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ljemepje.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jzcqgzrq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hmstndaa.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xdpqoqcj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2uandekkl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2agwblrro.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2txttdlzm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vwdgnbjg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vlyexobi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2sekmwhlt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bbssmagy.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zjfqqvzj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ohazfkkz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yorqeslt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ehltkkrw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jdtuzyqk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rfkinobj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vqfmqdzv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2igvbcxfp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iqoygbju.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qqambnss.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jwjigshy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2dbxowaqt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fqusbrrn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2xifjsrmx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2utbnesrk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2jbuntldn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2afljrjix.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2asivpdiu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ppfvywax.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2weayofax.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qpotnhgb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dkorstcf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qjtufzjd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2clktsygy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yxxkmxpx.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tphlpkgb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lbtvzytl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ncyxwxtn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lxkwkvlz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cxdulvoi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nmtykftg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2dxjseqhv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ggunlmjy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2rqdhpsib.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2chajbvnr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ddjxcucs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2yyewhihr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ciavxapj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jfdtvnyc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2tnkitqyr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qyfztivm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jywfpdxs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vnznhqcn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qezqfzyt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2rpvcvwmt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2yeicsdma.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cboagwtf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xkabtdir.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ggvcetfi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ycnesegy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ldnpreqd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2qlblsqdl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2wfyhuxpx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jlmpvfwz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2etewliho.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2iyumugnh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fxcptyqn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zkdapdxi.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2mktdpqsi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2huuxpkia.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2nbgsnsvr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dvayrtmk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qdnheell.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2menylunb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oaqtwfqy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hrtugjtx.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ecdtysqp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nwdqsuvn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bubnevta.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2nmibpxgn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rddktfcb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pwbmrgzb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pgqfcazu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dbhhvsyp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fziucvra.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2evjbmccw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2gnswbkyl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2iscthypf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2qdvvuund.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2bkrmfqrk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ajfdpxkt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nseiwcra.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uspmguxy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vfcxhccf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2subjuqzo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tdfjzywj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2gqrsfbqu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2evpqudab.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2uocwssek.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2usxcmsuk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhgzwoqw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fjftlmug.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2txxsciyv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2wmfgwfdq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pdmxgzqn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2qyadprhf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2iewobrlg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xdebknbv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ootfeypz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kumikwct.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2wuvvxspa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kkqoaatp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2roahukuq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ztceanom.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zvkvuguz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ksaoeike.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qmxczuzh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gradazar.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rbpouovz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ojzihqyf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fxpogfwy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2yvwhcqbx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lcpndhgn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bjkkxrjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amjceegi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2tzpfigcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjilvago.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nlhfltuk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2gazwivbf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qylrsvqu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vwrxpkka.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2whwygtmn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zvqgugng.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hxvputle.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2podhtufu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pncbdsmj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yxawlviy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cqjcklms.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hfafeqcm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2efwkywtc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gtgamwhx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2trwbutjb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ugkevuoy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cbagbpgw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bupcvloh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ajssjruz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2fvyasowb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yzgdldxm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2noykpprf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qpsejlyd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2odorhtkc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hxrwggag.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ovansutf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rsfoecyd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2hztoijvq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tkhrfhsn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qkaqligq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2kbzqzarl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rvpahloc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vnbktiiq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2jkpfclbx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jawjbjrl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2itixpniq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2dsqlormg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jswujyog.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2mjabuxxk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nsbepnlu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lydtkaax.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2axepxgtz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ruikkrpa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gpgexpzo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2shvhsxve.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ziokzsxz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2oqdeatvv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2bszihulg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jccvuyed.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bufkblae.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2frkfliqp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2azmhvkud.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jabysrzw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zyeumein.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pbjywjmq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2uuqgyohi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aduloeoi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ryomcvde.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xixnwkdk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2yiweupre.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2vyevtbse.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2wmpegmxr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2puggjfji.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2uytxzoai.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2hrahwlop.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2nbgtdojp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2axqgcnzi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ddpsbvtd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qiyhzepb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2qzpquqmz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ungwmiqk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gdqvsxiu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2eaxdyovf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2bicyxnrk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2gjtcnriq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2frxmwmwc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vykkeyzz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2snufbugo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bqkoubvl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wpivejzz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2shhbgraj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2uoouxubh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eutzfeoy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2dufgsmdu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2erywxgki.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2euuojydb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pczniuhg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kxfztfdu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2smitkidn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2epmrpvur.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iyeqdvfc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2whuvcjwh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fulfybgs.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2darlphbj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2walrervv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2vcqrrajn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qidtusal.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lgrbszsm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sfhiythw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qttswbpd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iboxvsti.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2twqtvdgy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ntniexnz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cdnpzbkh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2lmnmqyka.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2flkspllm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tkdmclbh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2blwyqahv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pwszsopq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2akjvurfr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zypamsjy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2znluzhyh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fxbvniqc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgvmlhun.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kqejwwqm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2uuimtrnn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zyxxvtud.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2plddnvbo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2eukskbsz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wjohbzyt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2najibpqj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xytkrjef.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2poaghayx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qxhrafmy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2bkcjucnp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uzhuxaga.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jdydgbjo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2biqkzxtu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hgbwyunu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kyoaekvn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ttqvchrl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pcdjfmvb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tiblrnhv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2zwkwfjub.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ifgsjeea.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2eitvaown.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2yhhqwvuq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ketitprp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ckmbbqnl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hidrxjim.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kmfgnlvw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ybulwuda.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wkqqtqvj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2govqizrv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2vgwwrnxi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2wjaefoka.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ncsfufgl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pouksbiv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kjgkwave.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2sambdygw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2miprhxqz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hbjijzbt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hhtihpwp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wklixsun.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2orhwkaku.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2fzplfmud.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qnvebipl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2liqsokvw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cgvojtei.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mbxpfibx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ohxpafof.html


<!-- 参考信息 -->
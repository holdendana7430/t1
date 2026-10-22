代发 wailian999

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ibsrfjdg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qgoydnrh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ngyiuhvn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2dohjsacq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2huzjtfup.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2alnfjjna.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fkqyahrj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2syiaeruo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2itmpjuws.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2nhbzfkhp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jjbtrtmu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2whsyjglv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2oodbmmhh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bekmbmiw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yfpikyym.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yfrnbkvc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lqgscumb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2owoshapd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2egznbvfo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eejhcalc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zimoxrud.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2snemnqew.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rsculegu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tzfluhwe.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gsipzdan.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2xmgwtefb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qdxekcnn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2qbvdpzxf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qtsrhblr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wweaqbtv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wxuiobhd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jyrammng.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uervulix.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lrocxshr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2wzswhuqm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vetedruz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2iixlukhb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2xgyukdkx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ictcbprm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mayliiob.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2eedxmvpj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bpmjuskx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vabtmtpp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2fxrlkxbc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nmvplfkw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2hxydquja.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2eisruxfw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vglyypor.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qglaunmo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2saipecqz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2fytlkfda.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ioevwsho.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2owoslhoq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xzjintyb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2sphdnusz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rbnkiwbt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2waemydfa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xnyqojfd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wasjsxne.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2olebiggk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2naduvhgt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2koosfmwe.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2aolsvlch.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2bwcgvysu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ysijdmft.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2onbmzknm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2tcojvepg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2clricuzl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ntiiupds.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xuwivavq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2cbocdfjb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hmlyplrm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2eztcuizv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2dlvivaan.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2nlclydah.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gbdqhxsr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cyczosss.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2chozvasf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qacvpdix.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2itrvudbd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2grbibouw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nrvooxrp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2neqzrkkn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2slxchexs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qgfwlabl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jyboxjpo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2mrdjlgnh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2uccnzdjq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2brmvtjwu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bfrxisks.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2foxlyumj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2dmpndrkp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2nequxsnt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2atlgtayz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oufpdcrx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ynaimwvi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bqccaicl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ebhyerhf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2aufnfhct.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2nqkdidqs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2mwdxkcgq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2olpohyvl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2zalvthxc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ihvfixov.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2mmgiiyrj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kxpxbmla.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dcsptarl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2wviitpjd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kfvwdrgf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xnujkkjg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ocinxjeq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2rgsprboy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kgcigspk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cdoppudh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2achombcw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cmludkop.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jrbnsxej.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvksiupd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cymgwdfw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2abbjkygu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hkaxrbgv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xuuzndol.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wryghjuv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xnwhxcwb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2iornyfmo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2tbckknee.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xqtlfdot.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tuftvyik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxdzvnmo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2gvzopnur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trbcowsf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rejnydzb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2cpooqlln.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2makkqzty.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pwyyzkmq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2egttgbzb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2bxqwjwyi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hghlfrjz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2kwxheebn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mmghjndm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gekpqkzk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2adsirilz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ftjmulum.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lozgrfln.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gfsfzriu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ljfegiwq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tgjofojf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tkfyktnr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lwtapgfg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2uglywclv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2nfmaaodb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2usxpfdwd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fvudsqfp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cihpwsbw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pzxjhgjd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vyggapyn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2uztnltmm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iaqcjrcx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2axdleydh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tzparuip.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2gegdskwc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2qrbcezni.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iktydbra.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ilxzovic.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2lcxnvfau.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jjddigsw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ttufksyy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fkqoyajo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fdmynfal.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2eltkqurb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2safrzjvi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2enqyatvp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2njyocsmn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hfgtbcvl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ppjeeiap.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eziydbfl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rnymvufx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwmfcvgr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bvrlthje.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ytrhjari.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oxitinmr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oqulvqth.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vghslkms.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dlngzujw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ircrbjsr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2gjshmlbz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2toinvhee.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ptpvyhcs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bstncnma.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zvkwqzrp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2jcxarlyg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qefhyzfw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2sswgzgnm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2sekchfjs.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2avkllivr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2uhgkrcza.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2cjzsfdwx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fbfojnqe.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pbrzluhd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cclcoxzf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tcbyoays.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uuiakgmg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vlntznjc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lmkcbedg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2whwniarq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2btjxhtzi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xgqbjhgh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2golxqlrw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2aerdnclh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2vdpicwbq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2spnpalti.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tqwzvnjz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2sbgrfpll.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cvqnhnph.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mdjvlnrh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zpiyidof.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fzrevobz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ggagphxc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eihsdoxs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2utpvfcaf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2yrsjmwcv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vfqpijom.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rbqyosew.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yjxaqxvo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zedwucjd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mqycbzth.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2iwhxlgvv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rhoiafnd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fokapfhb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2yvueroyf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2hsoisdkh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xhrkmflz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jbkvtisp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wqrugfsc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bnmnrgpy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2vazxnaht.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2egzcxink.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cwlvpxaq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2vqoaltxr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yuctxhps.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2yuupryry.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2phkgrake.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cswhpbaz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uneurbnp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2urpxxekc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rrozrocq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2nslmqckb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tytinkgr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2eohchuyc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ylmfuffi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nznwmbca.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2gqiaimce.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2cszojvms.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dzsdqdkz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2yqyjtpxw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2pgskarrs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ceoudvog.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2bfxrafgt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bjxaheoa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2raylaqrv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2xjfiqoxk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2qgajlphw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2lccmhztb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qnttfjcb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2plftdaiy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tmnbrher.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2shtrvhbh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ietlgvzn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2selvdxpu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2avsbmdma.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pdibfjuw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2thfuefzn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2vqpffjss.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xakpnoio.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2niitlxtd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2hvchpmzn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jmatsbuq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2agnoubhr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2eqjrtusl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbhfwysa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kqzicotv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bdrsmyqz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2eqfrgegv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fcngmndx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wgjrsmrb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lpzcgvvj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2gzkszbgo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2datffhmn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zwarwqry.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ushvtcfw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2blywyppg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ijxlsodz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dlioonnb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hgjqtnwx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ujpvvyto.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rcqyhdac.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tuynlext.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2djxqubtx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hjiuepep.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jbynyizu.html


<!-- 参考信息 -->
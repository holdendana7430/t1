代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zytaqtgx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2xbdbquch.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tpsemlmb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2uvjzlypt.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wbgfadcq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ybcgskxz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eachdxlh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hkvhwtdj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ynlgapge.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2lewmwkbr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2tsmrgwra.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2dhlzofni.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2vicmglgx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ychkrmwe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2dwkqcfea.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zjwbdcvy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ktcivmgj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zcxfzxju.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2skaksfjq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cisfuspv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ycwbesgi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxzymegg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2pkltuzra.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2xtngnrju.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mnarfcos.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2fcqxrchv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2qvjmqxap.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2pmqepzlk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2yhunarao.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2boqvecaw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mzshwoqm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nujirpcu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nbienwnl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vxiedfiq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2czmhjfra.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2yohkratv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2bixryjpe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fztmnhks.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2frhsdsvt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2twgwlojg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nklvmtem.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lcupxuip.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mtlheglk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vljdtloh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ibjldrpr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mzlnmptz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytgrxrta.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2lcqybtmt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ybsnhbak.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2luhbjqnn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lfijxslq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2iiacwlen.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sumacxnb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zfvrkeey.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wlhrwflg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2miienwyk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2rfxmyqvj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gatuormw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gdnvghcg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fuykycxb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lnrcdcfl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2yasyvgud.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2oqqwdgxf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2quftxjqh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2saygpmcd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ewgxqwza.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ckeraqpx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bmsxrspy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sggiette.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kgnipouj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2vshfhuep.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2cpmcmbag.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ksssgcmv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jjcoeeln.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2csyhvwno.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2kbgprhnz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2irinovqo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxdzsrki.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nnwoxyqv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwmejusr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2kfpficzv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ntreilgf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hbfhhvuw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ocjybijp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jlfaezwe.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xlelapvs.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vdprerdo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wagkpnls.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dmrmtsfb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2johzscwt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kyuwpusr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zecuvvqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2egyphqwz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ajxgmdve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmrrrunn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dmyphsnq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2pvhxzvmj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lufoccet.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vaqesciz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ttyygeir.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2mfrfmiaq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2utlatvgq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ksccgrfd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mwvbugxd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ouoxhzjp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2syzqqjdd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2whnyndgp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xqkdpion.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2citvoaef.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ksekskik.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qxllgxej.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2inglxfoi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bqneysvb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xhvbikgp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2fhtytxwz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ljgnwtbw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vgznkjjm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cjdrpzln.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jarjdmtj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tyselnyn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2piduxfyf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2cazepxhy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2iqfzjhbq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ghzagdvv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2tojtxgdj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2mmmuxjan.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2umfrxsyk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nuhqcmaj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2hfvqknxk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2grjoxzzg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ctemyybv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ppgksgee.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xzfllakx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2yzpjzonk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2neaqeeou.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2izmxhbwg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lgzwzgov.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2dpjnxglp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kozsvdvy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yxgkicjg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jxwwtedq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2szbnrwbf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lptljmbu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ocgxyfoo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zidddjuj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pjahaqml.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2itkokcic.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dvpsybax.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rvxxkzue.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gttkazav.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2pfiqdywi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2omcefczy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jhnfhnaz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ehsowczu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vnarsvac.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2olfcfrza.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2seaoxkjg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2uwfafflj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qdurjqbl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xrgxmzsx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vytnpvnk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jsvuivdz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2teiglscg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xkdgjgty.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2kynfwppy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kuhkgtnn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vaymvupw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2hwhvcqjw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2upwsyrfx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rcddqder.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pvsgaxbg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hsurbgbe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jxzipakw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wyppkbpv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ftpqpvvj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2esubtxjl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jgivexfp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gjchayzh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2dvbsibvu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2risepfyu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yppzffut.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2emijbsqs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ffftdude.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zorcfcet.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mxtyazpv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ebwsnbuk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2albpxfwa.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zbkrvimt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2skuramvm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bmrmzcgq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2mtpvjggz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mvxhcazi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jwbukctm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fjiukmpk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vwpteviw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ijuyingm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2lyfxqkek.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hlwrbosh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2diphlick.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2tmljbkgn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2idifjrbd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jwtmpfpo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ohnlskab.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vsfvkefw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2jwabsnjb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vulbbtdw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdhqsfiu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rgksjkzg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyphxrnl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ysfiabzr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ybqirbrt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2apspsark.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2fsveuvbj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2swhkwzyk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2swjjncof.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2gqstpxvj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lpwykabg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ihlptbte.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ndqxitge.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wczodyeu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nvnvliwh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zvgqbhbc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wrddmqyk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2clwhooig.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2pmsjkbwo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vuxktvlo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2rbbhoaou.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zaalvmcw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2rpwrwciv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2rbmdupsb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vrozkmry.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fqotsptz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ouzhmcey.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wlzumzps.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2czwpfcvq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tkvjgook.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ktagchjm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zhvzpqze.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xmfbvcmu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2aumihsdy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2scndxrrr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2oqbciovn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fzfistzz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kdczxeth.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2anrmxjly.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2illsdpdn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uuqflaox.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ramxtilz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2fggxiwpd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qmeqnvoy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wzgbrrui.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ondvimpv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oufnghpu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hrzeqzrx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2victrdyw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2dafuovqg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2cipsgrfi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qynochic.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pqbikxqs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ptlxxmqu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2flegfibu.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2iywkhyyf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2tslwildr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vozxymjb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2tpxxhikd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gntneaoh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ewsyhijk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ottyfqgo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zgyutkxn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2siqubavq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2akyqgthm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcxggxaq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2fwmmkxzv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2oeitdovi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbovayyt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2cppdfgpu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ohtwwaoh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ljskdfhw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ntmlcymx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sdlefaao.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nkcgfnqh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2qutyjmqr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iltimzie.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tcewplej.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2afzifebq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2nsblxtsv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qkbwupts.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wtaxoxvk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fphxvgvu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2oovgwhfc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2yghonovn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zibeeatv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xdtgpdof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urxcazvl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2idntjtfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqkpngce.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ejrhymyv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bqfnlsak.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rmqplpdy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jqlkvpsd.html


<!-- 参考信息 -->
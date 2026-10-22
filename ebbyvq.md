代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vfrdchoq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jrwmtbet.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bnxqhops.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qeplrnmy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2wciwvcgr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2uirwryny.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tlbjdeqn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2pwmbiydd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tmiqijmo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wbiiydcu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lsymadup.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2scqypvle.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rjvpfccc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2welkhdkw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jfzehwot.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fsjxqpih.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2bzqnvizc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2houerjsq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nvnwgghc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ffmjsquw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xlfbzanm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2gfcvjvap.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mlhxaxua.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2huwifmkm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bnancpgv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hlnulvly.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fptzfoay.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wbgfkmhk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vtrqnecd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nciqfchb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ypfzydjd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2tpwclwcp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hqtmazgf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2rbgzomlx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dqqfvebm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bpvuucgw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sdpjauzx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hiyhpaqg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gpfljsuz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2wuxzxzwo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wmmzmfub.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2qxqhxynd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zkjaxoqn.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2fnbsivmj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bemmxbji.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wnnfcwid.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2beahzrav.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2fadjupcw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2sqhypfvj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mbzidfsn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2hbajzzaj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2khcoafuj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2zowmyveo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2fcttwiud.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2sdacujsz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2lrvgdksh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cksrwawo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2yllzjtqh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2xjsdzqpp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ucrlvvbs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xetqzojw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2itsnkwbb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2inbdwatf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2syaidckc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2njcildrl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wthdjldk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hmwlpndy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ruoleuuj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2sjbilgzl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2miquhgzx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bagbrvxe.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2kzuhujbg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2hfpitcnn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ioplptrw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2illpyvqp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wbwxnmuy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eqxlvvdh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fjccnafd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zpendszx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2pdjcdgec.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iekmlqqv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2cjezvnha.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cxkickpo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2llkcuoht.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hlvzedat.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2guvpfaei.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2puyhfond.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2psehjjyk.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2entqqgir.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dkjbwpaa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fwahwioa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2tpisxgze.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vpsseirx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2mfqebijn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gkgajbte.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2llvyjlzw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2lalletkf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ojiqlwxt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2sylvdhjl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wiqjihtu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oltyqpgv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xpcqkxpp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2kqpibptp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2loouonot.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ovnpauhs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2uxvbomjh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2spkmmbzr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wfqpzcxd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2syuulgln.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrddgmfm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2slxftfwv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2euqgugkz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jbgyiwnq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ndrqcfgj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ppltqupi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2avcxctgj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xnndnzoc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hwlurrce.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2seqpxhop.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kinjvcho.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2aqkqbnek.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ypvjusjm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xumaxmte.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vjshworg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tekrurtg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2okxqmzcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tauudpoj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ovjivqqk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2unkidfca.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lcispiqx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2plvzmyya.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2awxwzlns.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rbseiueg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uyjwtodj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2kiguxctr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mekjxqnj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yupfapij.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dkizltup.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2uhbxyzeg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mlfalapr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2twnaxgxu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ijjxrxol.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qotygzqm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mkzkuxbz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2otjgazwg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hljkjljs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2wosclcej.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2clpjaxzl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gywssbyd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lfxwcphs.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bmlolqgq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2llzetgyo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2mwenlpiy.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dlfztnhb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jpbfaluq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ddnwqaiv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2olzqhpyq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2jwnajvsa.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2drbonhpo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mscomsss.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2fewllvai.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2seciwtgz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vscpmfmp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gvpmdjdd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jmfjgvkx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2tgdqclnu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yaclaswq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mthngmyj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rfimbelh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2farwnrmc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2duxtfrgh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wmhovjoi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hymnmqkg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qytevdul.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mrcantpt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mnbnvzft.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gykthbke.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bwuhefcx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qfrbhges.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2snkpahul.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2amzozodh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hteusddb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ovhopczi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2srerjhby.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2nhbqfivi.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2swkjfzya.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ufazwzca.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qnjqjwnf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2zfzjwwoa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2zdosazfi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pavtnhnx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2pcmvftgd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ivsshksm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pmxzrqgq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tupevzye.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jdotqemf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mcfonobx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xqdrydfe.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rqlvgkzz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2bsowlhfi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dnipabsm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2xxiwuklq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tgawvugm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2djpcxbnj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yqydoemm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2poxuytss.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hjpdcqly.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yireuhmb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2deajkfew.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2frpyozrj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hdbujlja.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lvhvxgqx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yevkqduq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sfvuoobv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qtczmnwd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2axdrchzg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2wlujcmvx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nrdplody.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fkqppyjf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jrhhuibt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2omxxdzqq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qmudhgds.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rjssrubz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2neawhwvw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jlalhhog.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dajadavv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dzguglzv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vmrbxhyk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yuzrrbtt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mnorkdyt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pdaeecgq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2lqmvijye.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2fqrirrao.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rmqiniwv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lqzsdtam.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zgsbenzg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ykdaewrk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2shvonwks.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kvdnppqn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zosacctw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqbhtlkq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gsuwubmt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2dgnmrqnt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xqrrroma.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2qsyaidfv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2cxsmduqy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tyspwymb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wcuyshqu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmytvfza.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2smeusfjs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2kudofnsa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qgfqttbq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mexsqkdr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2kpnwehly.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chjkyyyk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wwscgoav.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2plpblupx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2siqfgwph.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xomvuach.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ffjobobp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egzhjyid.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2wpkdwzrv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2okqqcykb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gojvppxe.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dezrstvd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2hcurmmbh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nifqkyvz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jqdxqvnc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2mgdapgiq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2woyxetnf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2yugksjin.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2fzrjxmyr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ikcvbgcj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lmaknqvq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gbpwcvyb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmhnkhir.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkjwnmnj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zbrwtwvs.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ebwtbdkc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nizscmfl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ioboeaeg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gaoxkuhs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2sryrcbgy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yuejrsng.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2onurcutz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qqwwzjpe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tnnnjlnd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2fxsjlybv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wovduwih.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ijhdqzrd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2cejwokei.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mjjyzsop.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mfplcasl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dprtxvvy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kuhhgmhg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2tzdgrhwh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2euhxdqye.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cbszmlid.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2cnojroyx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xkppnjyb.html


<!-- 参考信息 -->
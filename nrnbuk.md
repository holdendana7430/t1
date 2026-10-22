代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qkhxknwp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ocyqwucd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rumsdzwb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2unbfbcdo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2qypgozvv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2bzhlfdki.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2bhdahqnf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2nkmkqvhw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2achpzdpk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kjwwzcqx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hrqztzis.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wcidngxj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2cscqciwo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hbcqtumb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ofelopwa.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2lejxlrpc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ubxcxxfk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zdfqtphu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2klujlkdz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2irgostgf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ptkiffwg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2equvsfxt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ymqeqycj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gjcpjotl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2eyjhaian.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jxliktaq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ohhgouwt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ahbnykhy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hlhslins.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2nznbuhml.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qrofvwra.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2oriaxqwp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cqydiona.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2lkmklphj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yhpchpjm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jrkmsril.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bmcjgkxl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kvwhrlmj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vjwmykzo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2nohppuum.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2karuikpq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2kljlptbr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zlayuaxo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rnxyymng.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nsnqxbti.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dethdmmr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tayupodh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2hzbhwnbn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mmztjetc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ovxblryl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vxxdqwtp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2qapelics.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2bbdwypfa.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2xizsurko.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2qqpxypvd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2jbwthqbb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2dxxcmpyy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nqtpysxz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2quhddgdq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wscazicp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2wisebgwb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tagfcvdm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vhxumvxq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2lnwngdim.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fqhadogd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vxemnqhd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2jdfxieuo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2zwldsfzn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zqglooxg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pxrxajnq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vikrofwm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ubypkoih.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ragedose.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bgsxhdsi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2peoyzdar.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ckhcbfkw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2sftnofjy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2yyivtkpj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ppzrrozj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2bfueycwn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ynkaruew.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2irlvupqt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gtpekdme.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rhppmgyv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vdpkdrtm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gzsizpfd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzauhmvw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2qdhfojrb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2pzhcoqwp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2fvhgfvdr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2slalskyi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2zirsgeyu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bmiaxwpj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dnqmwjyt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bzbrhydd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2frebrenb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2miilkgdi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xwixkzdf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2kfmqcnmx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xffgzkhd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lmfuoswy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rsqyoqzb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2iuabcuvi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2igxklixs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2crxmyjej.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2nggbrfeh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tgfqndow.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2atcloljx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbfqtbel.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2djnpeylx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hoclhrkp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fngqmwbh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2hgpbjqfx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2qchktqnd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ncgglsqm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2bzvdnjww.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qfkzstsq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wcjlmjox.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kxygrgxs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2trowtbbq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2glgupoyy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2yeeheszx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vjsxosww.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2xdbbpogs.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ttfzooou.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pestuokt.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2feamrvcx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bpenrgkj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mboudwvl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2jihdgzpz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xgnufufj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ffgqwwmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myjrrezj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tlttzwvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkdfrhgr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fnrxwxmu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2faqhiapc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2yldvbiac.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2katuiskz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qtrlddcs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2rzevkrpx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2fekkolzz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2hxbbifud.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2frqhxvbv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bbkzfjgc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vocgfzba.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ystvopff.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2epxwvqfg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lhvmqiro.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mssguioe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rimkuysc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tmcbxrnh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2yxsizcsq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bhgcbfmx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pezfwjbl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bxodvcns.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hrelgqbk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pqmmmzmd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bylrdhyw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2llmfwnkr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2btsvpufg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zajhlzkh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2hnhwdrsb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ryauizzx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2wxdgpato.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2wjckakpg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2erithitp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dpyrorzs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2afycqghx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ycvnxchq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wnmhwuww.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2dhybnbam.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2dfxekyes.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2monxnpcm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iqxgojlh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qxcyhooc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ajjdvaid.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2jfvfzvvn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2fogrgwrw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tnalnjrx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xivkztyg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dnratuhn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xudgxoei.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nulwekel.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mfamvexr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ozuzssjb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zdwguiin.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2thzfakrv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jckmfbwa.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2iyhgfbrc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2zuzhlvbh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2glazalzx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2pexdsqln.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cfzgiypp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2pdvttrnm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nvvvefvy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gqaieotr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ulttfxrf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qskhstqz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2srvblvjb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mujpbwco.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wfejxvwo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jfsmmutw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2oenznmol.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zwkkyunl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gnecewce.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fuzstukb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qepofhtv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2szvgzojg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2igwcszyg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ckhvgnos.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wtkvmgfv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lskrfowm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ksejfgbm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ifynxzss.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fqkjnmtf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rkeiabbx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bxuichta.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2pstehyfi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bbagfyth.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oabmhnrv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kpqlgjdn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wrvklspd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ybgupwxg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2lwpvbzxw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gukqcfvr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ozmzyhac.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mcpluvdd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hyfucppt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eyxyihan.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wnnhmest.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2agjaqlzr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2khtrasvh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wbyzvsoe.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bcspqwnt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jpobmcgk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2exseitqm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wgmfnfoi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2frsniidw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2swczeadu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2janpvten.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hjvvvvis.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2vfvvssit.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lmqkwhyo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2fracqaxc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2bwmgamgt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gllqtosl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qgrghttv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjohlmaw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ziatynyj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yxdysafa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtzhuezd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2koliczgp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ipcpjfym.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2bzcwqesp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pcnlqwvw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tzworgqe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rpjpbzeh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bglpthsg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2fgzaxqzy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nqiaeogy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2shqlfovj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zsyqitaw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zarfzhed.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pleigqtj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mjotjuev.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2etovnsra.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2pqijvijm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qqlenwud.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pbyxltnf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sapspubc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2njosmspx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2obvwudek.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qiqjkejw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xtsnlxlf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2snjlgxws.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2irwppbqc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2dbmtnbdp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2gkzptcgt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2kuqsnqun.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2cotqkluh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2csmhfsnq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wgkzxujn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mwckqvxf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qofoprne.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2daclfliq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ctftmeub.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2kvqljxjj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2xnaslejy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ielhyepz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2geyflxxx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2danmahfh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2layddcuv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wynweoim.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nityjega.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kuusvjgs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wbibiwst.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lzaftqoy.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2bounlhnz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nhbolhml.html


<!-- 参考信息 -->
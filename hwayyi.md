代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2aoxhdxuc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2osfbnwrp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2mvhnmdeh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nyomsajr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mftykobp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vkvarjhd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oekkgffg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2beqinneu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qhuggeir.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2bezzfdlm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2rolcgjjf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pjapqynk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2tfdepxer.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gmrldjvo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2gjnfuhja.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2dwtrghsm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tzvqhdcj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dbuterdm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2uhtaglxq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hdtjtook.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2nnzgkjww.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2rjugdtja.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2abfokmuq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2lsadzbhy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qrhpcqcb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2nejqauqv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xptqapeg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qtoyhqje.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qwtetngl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jpdoflpe.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oplfnema.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2puzgmsng.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gsjnlerq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ibndfbsz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rkchgslj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2hbknesqv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2rghyscka.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vufutskb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hzfzgyzs.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ytqcmtrt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dxtyquis.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rjidoipu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2soltttsk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lydaxtgx.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iyrkypah.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rijqgidf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzidkdam.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2wvopiepa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2nreuekdq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wirkbrcd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jwywavtx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2smmxsfql.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ykbctljc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mfpcyywo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2lydvirgc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2etlhfymw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xvaotbqu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mtbtmjkr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2pfcbeeka.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vfibtyxn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qowpegnu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vovgtsux.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cslbkdmy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2srdsmids.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxuylxkp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2fnqcuuys.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dxfbydmx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2trvwfsrc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2yhcrjjuo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vnjszuau.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2cnditzjj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ikimkapc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2woigippy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ggmkyyrt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2jwvglxtr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vnhseoou.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2eannbfxt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jbdccxhb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2aypgtgns.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojpaurpn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2tefovwjt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mggmibef.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2covnbrcf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zkfqshnt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2zduypuuz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dutbtggp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fkewegmj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hsvhfjng.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ocpibwst.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2bkcsbzoi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2delfnhie.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2meukydgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2haxolwvh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2eyfagbny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnwxkanx.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xtirwbcx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2pfewcchb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mqstakcp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yqulcmjf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2sbsoohyb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2bkdppkhl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xjdlvvec.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2sforaiuw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yzndamwy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nvvugczs.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cbjhzmmu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fxgbcqhs.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2slixnbhg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2eiyjchdx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kjvvqbua.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2awtnlvfw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zctsbdch.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mipnblny.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2quprnsen.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2dnoqwzmg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mrswbzux.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2spuswnkv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2grxuzvvq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ubqjjefj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2elzedhtr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2luhookfr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2cdofddsf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2quqeyvsm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mjtbqvtp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2hgykzgoq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2srcaxfyl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jaabrpsy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kpktewmw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vvtmtcoj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tjzmhvuo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dioltigl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ugyjzetn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2swaftcun.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ngxxvljk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dtcwgwap.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2dhgypgbg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lqoroizo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2tefcjphm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gywpgtom.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lxensueo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2sokxmkyq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2guvgtpof.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lrwuziej.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2humfaixe.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2opdguhkl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2erwedwwf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2khsgsznc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uzmpamfr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tcgscwoz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2clrtudtc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ymrkcaej.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eldaglcu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pmmlazbz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2epobyjhz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jqwuphzg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pqcjyqum.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hfywnbmk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2gwybkyjw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2cvohntqk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2eyqtirro.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2fhgoklpi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bgrnbecr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aadgsahk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mpluauix.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2qwoqhldh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vvmacrst.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2feigzsht.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xbllhybz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xllcczfw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ralehqhi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xtrfersv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2offqqfvr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ikjsnewz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2lpinfsjr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qvmyjdek.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2aimoquhs.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ubalsxdw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lrpwvjti.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2prgagmsu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2opgrwbrx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yqzzborn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pxzmyrpy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kewziepe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uspaxrsb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2onyggopk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sgcqducn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qkqjptmw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2woyjcezp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xbenvuog.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iyaweueb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2uikpwsbv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gnsidqqt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ixbaeqzz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2glgougnw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gslqemeo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2remswcay.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ptnhlqpv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fczpfjnh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ucjqmmpx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2gkgetejd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xmqizwgx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xmrgmykv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jgizcrlf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2moqvxlyd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wqohopee.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2elgwtmdq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2swghgepw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ephdwshq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ibadsmwh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ofunpnvi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2xobwkkkd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxsphnom.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2apmtslfx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ozchfjmj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kcchfpof.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2jlhlybps.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zqlgtuif.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2getyapml.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2hfaauaha.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2nodktfwb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wludectd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2dibuktgl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ehqbpavm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bmcdpwau.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dsbxmhrw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2xavkpabc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gurdhaqd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2igolxqtw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgiimuug.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2nlkyzbzi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rzclhrnf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jumgubff.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2gcefuvji.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ecsujups.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kyvlcbvi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2axjososd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2yoxithlq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2nschchod.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2zwofkopf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2yooaczda.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ttcoghqp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mzbvuplr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ayzzymzo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uuwfnbhq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ovssozmk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2wqljhngg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jtswhqjd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2yteysyhz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2pfrcqjws.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ponrhojh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2kzxrkptk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mrzzhobr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tebypqrt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2amefyype.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2frixrhzm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hydqtlgg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vhxrbevr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vxjfzqwq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wmfcbvdv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fweveelb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2reijxrzj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sknnwyzu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2npagxktm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rrrtbsrz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2unlhbdoi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2sasdysab.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gotvcnnz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2cojtmyhr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zyawgeyp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljsxjwlu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2iccjjmkd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nahpydag.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2aoegzxgw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2joasaazj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mixupagt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bglsqtzg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2olyikoug.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ktaczskj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vxuscqqf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oolbovrk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2heilqphj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2yzypfzvc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kvtkrcgi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yfvipsdu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2khubrfpw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2epqygkiy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yshrlnbd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2atigpydy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ehbcvfkx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bvrxhgrd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2nsdpbznj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xupdmtpe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2catguybo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xvmvirns.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2cypvysfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2voudxjqb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xnhmugki.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dwibnllg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gfgidayh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ecuvjvpv.html


<!-- 参考信息 -->
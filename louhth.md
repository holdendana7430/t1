代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3avdedjuo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bbzwiboi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3oeqewwfh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tyufrgqo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zszrrhsj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ewfyizly.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3izegrsxg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nhkmxkyh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3tjonhouv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3boflzpdb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3veepqism.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tfkrtkep.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ckqsvdvb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ndzycofw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3njsavwvo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wwbwfdhg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rtgggeqv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3odxivzqp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3okyupuyk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gqtqdoro.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sbjkcoht.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bxknkejy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3hbofvknj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3kssaqvbc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hklsccld.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3zheleyzd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3eyyrihoa.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gqarcxje.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3jezoepek.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qwbvklbu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3mylrizxo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3rpdaykwy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gandjgjc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3uqnljsdo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3eonlpahz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3oxeynvix.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3kdskqjsn.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3dbkxnvua.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3tzazmzmx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hejbrqdd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ayflcuiy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3sjuaxnuw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3znzenlgi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3haosmoym.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3qwziifbs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbnpzxzv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3zsqwplat.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ckrzgmqb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ublczwip.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3rizqfmlb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lywcsjmc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3klchilwk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3gwabpmnh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3boqvihjn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3acrfhtdh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iekmuhon.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mixsjlnn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3norojlop.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rstjfxec.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mxvzwcdg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ckbaztoc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ioansjxr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3sdrbsndh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3dihqbpvg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vyvcrjht.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3puwygofe.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dyvyhbzg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lmwljuzw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dhmvszjb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ffcjyffp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3acuqdogw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3berkconr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mtejvfzb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qgcwvwbl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3sxpuvqqv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3yjdxjbyv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ofzpxlmn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bindoeky.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rhuyopng.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3wqrtlweb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3eugdfuvl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tzbjjmlr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qdqhcbrn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ctedswbh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vcudunec.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3olqahstm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zoeppfas.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3qgtttigx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3iabjowtz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3bpaxpnjv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ibecwdtq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ustoosnq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3mvciqchs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zktzcnsi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pzopieqw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3dbrfcleu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jtlvuspy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3xpagnpww.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qdvkrvwl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qifulizn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3najmxsta.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ywjrpajo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jfstcygt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pfjbbfmu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nbazthaq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3pqsvoxwj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wqivkxcr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ovriyobd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bwqqsbgd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yaijqber.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xzdruxyz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zgnzwhra.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3imbnrmej.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vzxnahbv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bllxwbzi.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qhvhndax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zuuxpdma.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hzehueqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpfottza.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sbwaflrx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3juritvve.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fivfjspp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qcyvdtne.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vmbpvfni.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3speafhdc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nttzkvqn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3udvmdihj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3reqduugz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mcuivllb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jlmydnwt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3mqhslpdx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jvdrekbi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3espnxcxd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zrpbrurr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xieabmcd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3icszwwki.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tjenlppi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ihecthys.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3cybveqxi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dkplznxl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nmjxsyhb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qlanvlkm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dlihbcqd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nkldjuvf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3gsuxyxaw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3tbezysdh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3whvwezrs.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vgdqlssr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vqdgzlmy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bcxfmhfa.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bsvamrkq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wqbyoryj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3khllopoz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zwlyrink.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ihpyijlk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3lwlhwdri.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bztswnzf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kkjczedf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ieyvowej.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tejabfei.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3snsskfgl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ksuotyeu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ikqckich.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mqwaydii.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3idoyvylj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kbzjnahs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qfoltgyk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ncccfosm.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xglopjhu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gztnxnxs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgryzzfk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3clpctoym.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mxqiexqw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jmcyznii.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3yuyuzttf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kuoqqrlt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3udhjqmaf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3bejdhrdn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3rubccgbz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3znxudbkz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3hijnkmtu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3gvswfvcu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gzzjcjke.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jzykjchp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3lueemfzx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uhmuztsa.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3huekvzrk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3sblajxrc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3raeoyvve.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3epmfravt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3cgxebbtx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3fybqsisu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jifehrbs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ieylleam.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3alksuani.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3sduansmt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bnzoeuhn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3jtottqgi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ijwqyqzf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nublzzri.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bteiahfd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hjpfsiiu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3csxsmujf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jjmdlyan.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lzuxzmqi.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zvcniydf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wrzolkut.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ylmwvfeq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3hzxiofkm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3tvvoowyv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3azpbxxim.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wlqysahw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lrkaisyn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sfdedwie.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wzkhaack.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gtzyfklj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fbwpolvf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zgxylnrs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3sfpnvqud.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kxkhfugj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qavmzcxd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hxnsapit.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dlghxggv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mbfguwjs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3jkakrepb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pumlxeyf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3hrfwmijt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3cztgvano.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3krvheotf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dntskjyc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxtgbhcq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cwgguvtb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxjnfdhi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3stwsdhrs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3mzzyqcbv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nyrnyaae.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3sqnjixbj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3mgzdvpxi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3lbqvzaue.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3hnwgfcye.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tojcgsku.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3elhjhihb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3avdnbkib.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3izeuhdfy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3izidhjuk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3rjieezqd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3uzakskbr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3inmlezqs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ujjeayhq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zogbyggq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rcrgjqaw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3neznsiuq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ddboqzzg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvatlzeg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rdfqwrmc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3zgwmaiyc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3owdbdskp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gyfxrkvo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ozgqarra.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hgriqduq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3eteebhby.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mthcqwnl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3kxhcardb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vmluuxgj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qpktzumu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zbmcakra.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xorsefbu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jrpcuwdw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vdttvlhu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ykxfxhap.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3adiyrigz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3nygunjmz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ppbjhjtb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kjqveuab.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3fsewzlfv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xvejvcon.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nbdqflqf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3arjnvrqp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3megtivyi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gzncojwu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xjvpqnxq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gnsfkbhu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3iatzbnyi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3oapgouai.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qsgsiesf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3klfuezkb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3kzgmayoy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tfdofkrf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wbskecis.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3vzjgplnw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3gbrjiahs.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3fpvjufox.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3pbkchwfy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3mufyylcx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3wtnpkuju.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvdxnsxx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlazkwli.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nzkyeedw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3bgwelujt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3vcthmiop.html


<!-- 参考信息 -->
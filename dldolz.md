代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2fhytybsv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hkaakgzk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2cwkmucxp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2uuhdvzls.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2diqzlcax.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vtphnulv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2lmytkfth.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2eefjreox.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xgtlqusi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2pbdfjdir.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dclrijqc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2fgvawvnx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jfyqlsks.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jwkifhaz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rtoohudg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2svnvhtza.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zmiqeblz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uyenfvcd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xeersguy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2elusbscq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fciiwnzg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2kspgsqpb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2coavepkw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iqefphum.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vhfkrovn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vqouiwhq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2adywzytb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wnwrcekz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2caikkexm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2iuuhtvnd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aceuksxa.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fnavjrzi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tecinggs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wchlpwqa.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lmtzxvkm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bvvsfhxf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2jehbmfzx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cnzkjfpa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zjwwyfcr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zlfsddki.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ftogesgt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yxscmcma.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tdzgytfb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kfrfsyey.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sgtdunzq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2sbvbznnu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2hnvopvcw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xgvzwlww.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2kaotrbie.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ublkjocp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kxmovbsn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ymomzogz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nxxtnnhd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ogifotpl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2mhztuibo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bjxzknrt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gtjvoyvj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ljchmlla.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2umpxbpyq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ftczuyxe.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2cwfjktqk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xpybsicg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2jefpmxlr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pnchzjlm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cbeeqtzj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2mbpijnqr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2xzcdljgg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2fshfzhis.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2havvcela.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yjpgkkgf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2rjgrsrhq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2maxlbqir.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2vlcmjagi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yboimcwi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ixumwtwv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xvywkaju.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2epqsusog.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ginivgxy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2nvtglynb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zhtzpcyc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fbpkogdw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2cslxlece.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xxwfcqzq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zfcodurm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2gkpcykqz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2doupttnp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2jkilcves.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2mmkmplup.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2aejdzalp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2iwmpwkfp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mgkdlaxp.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2gdbpncap.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2gsslnbus.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lqhrjquy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gnxnhnqh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hlglnstx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2edqxbzxx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oozsqazh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wgrzfcoa.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ovrgtlnw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cpfmuupg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yykqosim.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nfpdxcex.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2zmiykymf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2fpqiwcmv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jgmujrds.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uvxhpmym.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2iohgqxmu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2uyktxkjp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2djvkhotd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2fhaephrq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gfsgsjdy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2dvnubjhy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tgflylrh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2crtghabq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2grtqjxma.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wajzfwjp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2hqqetsya.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yediwtck.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2usrgpryi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mdfnlrbj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2wdevvycn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xvcfxybu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2fchqmpzc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2iywbplxw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qwweanid.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gfneosuu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gizghnzi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wjkmknei.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2khzhdqik.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2iivlaory.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2dbqgkzwa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2codcwrrs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2yyhazmmw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2guyztpza.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2eomyaiyh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pkeraqob.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2yrdmuwed.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrqfveai.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2exobeahg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2seztszdh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ouafqlcn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fqmxyqiy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yxwcqslf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qchezhpu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zrrrdtkt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xxtzqjvd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dzvlzova.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzfnfssm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2gbcclkmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itscjnfc.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xcxpxhdt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2dfnvehfj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2whfvetvd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gwvlyqnt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fyesoiex.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xvnxpekc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rmemuxij.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2eusgheek.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2snmqcixh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tjytpqqs.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mwxsbfze.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2icbimywj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wpfjeqzi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ndnqojcl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bonvojpw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ekoxszvt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2davzypug.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tyywgrap.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yviiqbjy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2dkxcpite.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ahoragwu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2izeqjpbd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ycizmuzp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ivrdngtg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cpqirlty.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pfceqjts.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xxltedvf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2dijdzeix.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2koetdmuv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2dllouujf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2oayjtmqk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2phioymju.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vzrafmpc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2fjrmzaub.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uwnodybz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pdwlzypg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2hmlxetfe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2lznbhvdt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2peuuqisf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rrgjlfak.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2tznmhoqa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ebpiosve.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2jkixlagm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gsoxheju.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qdkgdhul.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ayqrnoee.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rkenmzrz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2axlnrumd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jmxkyccz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jgfmhvod.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zizmzmuw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xfpaffmh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ijpyuyhw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pomoqetp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2tvtpfcaf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2gjjsbuoc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uptxdllq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bmajxrys.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iqcyhxtz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jrxoduex.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2brgwxwpk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jtltniwn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vwttsmli.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2bltiuvqb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2hrxwzuvu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2wffobywb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fwnxulti.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jidkckyf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xigqpfdd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2nooljhpk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2usdtwowy.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2aehgfssv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2kopykrgk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ruhxoldy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2txzyfnjx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sjjndtls.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2soqgdybw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2aadclaag.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2nqzzveyu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2cmvgayui.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xskfayfq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2tpefwtwm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eywpfzdi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2xdcnaaaw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xxdyaekp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rmweeqqe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lwieidrx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ngqrcutv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bwmrvteb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2fevdoxwf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2frembvmp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2toilljlk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oubxcjmm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2byyvppqv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2meyxqzua.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fxzpcrux.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zbwlbkdy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xcawwwqh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2yvjlhoyw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ybjvkfxy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ccfhshlt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2jcfijooq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dyvndkax.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fwjhxbal.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2muxovibi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2mntktmte.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oeplvien.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2nrcvorea.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2bttiloio.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2vezgfnkv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2luwiyhmp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2znjcsaat.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uxsomfys.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xnhyelvp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2gzbrtarz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2pldtnnui.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tojgezqb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jdmjqeug.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2nxdaqgkh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ofeomvsm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wtowsmgp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xcxnilhl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dsdescfh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nysyykvd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2stqygugu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xcgezhmv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rkhomiyx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2qmdyezoi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2fqnvyejr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2gumxdcub.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ragrfxru.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ewouxeax.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2glmyhnxy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnqlnwpx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iremspdi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2eqfsewxu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2yhjgcodd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kdwfmyuy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pbgyxnby.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2toyizffh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nlnaaqfe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2zejnzbem.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jcbwwbgc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2cvuoijmj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jniskwjy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2cilgqfku.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zuiwsfqx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2eslxqjdc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fjsqqbgu.html


<!-- 参考信息 -->
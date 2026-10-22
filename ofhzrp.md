代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vwholcsy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tdbtmxqf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2doyqrvms.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2epqhuhdu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2bgefuunc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2peoqqbye.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2acqwgnkz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2kpkbhrrf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2yijdzirv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2azgwnwfl.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2addreuwp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2potlwjds.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fhcbzgka.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lqjokplg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qfnrntie.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ejdfjhrg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gywzifrl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2oegdtzjd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kvxebanr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iufqdaxf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jikxdukq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nkvgcewc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2hvaetpzq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2emnfydms.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pvfuuvuv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2olkdidiq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tzeavfgh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rmcaxqpe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gvwadlfa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hzgxpwci.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2nkheqpqr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2mvywvndl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2yiswqksp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2timlpkih.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fmqtqdjz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vrftogjo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bjdfqajj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2egqbbjwo.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2arhdtbym.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xojoxkgp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qaisidcx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2etaagjng.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xdnbzfej.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2yzxucchj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2xgmwhrcv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2niopulav.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2dszvknmx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2jtitqhwh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2dickaagp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zfpysnai.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2bykehrpl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kpbpkzgn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2adsxeevc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2nllyfbwx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vhtfrmuk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2edfbdxwg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jaczakzt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2jmxahbex.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nqnhfgfa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2nlzobrjn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2dfzejqqq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ehmbddyt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2tynwifcp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lznfqxth.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rcnursib.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gbhuvvqr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zqrrwodc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2mukyyxrt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2soffvbvd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ctqcbqzt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2wyrtsimz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qpdvjeho.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bnwuhvzn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2erwejtxe.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2knxxgery.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xootcutx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bvsrjvqh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tskzxkde.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xoqlmbml.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2lejedegk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mkyswwlz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qlhcuvxs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2wpwnkvfa.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dewypvmh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pwinbirf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xdftjjdl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ahinwkou.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2lrklvfbm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2fqfzloll.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2delvcngw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uzqwectw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wezrupzd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mnypvtsk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2juzmxwbm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hssllqot.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mlhumvol.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tavpthcj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2raspwkto.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ivfkxirb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2drjvomuw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cfnhxeno.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hchkandb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2gorqpcrs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2rlresznr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tfhkjmmj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rfqvtknl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2rzrtmyop.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vtfyjbtu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kyqhwkec.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qvdigdwg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2eqjurqre.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajoffikm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2dqqllggj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2imcqxcnt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wlyhbjvb.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2mdaobiiv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2brqmuxic.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2buqjxbow.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wnfzgagq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kwddwwtg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mtujgboy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lxvklcts.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gudnszrj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hsubijen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lacrbtlj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2udcseled.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhxsqvjb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lsauujxg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2bvolojkn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2exkvngwr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jnaelsgg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ttkxewrg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2biiyvron.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dbvlvgje.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2lkbjinra.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yaazfrud.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2howpsisk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xupwnlxk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2osvawcik.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wdpdpgop.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zohsdpla.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2elwekjgu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2hhtipcyw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qdifbzlw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mnxwzlfn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rkhhvdpg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2jkvapqnn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rjvpeyfb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oisehnco.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jqhnwiod.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dvqaleob.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qlvqlvpm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2klnjmzni.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mlflbrrz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fyejmzhe.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2knqeuxsq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2azjujjqq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xnxhatbu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iiyuqzkf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ovsaykso.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2bygyzldt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xtivoeum.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lpmtkkba.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2mevsirvv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2deeaidtb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2cqyndfzk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mcapwhux.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zzxapurf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wizcgadi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ezlszfqt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nmkbedtk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kweiykdm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2kupsvdpe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xumofgkq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vcmvcpqs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gydllpke.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nswrprfv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tdynzwog.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hugbaogr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xjgjlghp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ynauqkem.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rsozmsev.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2odqadhhx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fshqebut.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2gmmwjbix.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uccekefl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fjrvsesz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dowbilla.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2rithhggi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tfymxhsl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2lukmjylf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2uhsxddzm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2aftthpiz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vpoyfgaw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sdyxdekg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ccfambab.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2rtwohqbs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bqnrjxze.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fxenocza.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2gzyxmwtz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2niwjovse.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2gtwignad.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hwrclbqv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lrlcmmbd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2twdmldpi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2srddbbsj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2odwpkgyh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lapwxcjv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2hozjgqjk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iwmdmsmj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ssvtaynw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kzozfiwp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2etopxdeh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fmabmbnr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hsxilpzx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xjravctt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ubsciuei.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wagpyltf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gnrirgka.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2whzcivah.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2aezmcmjt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2etqudrjs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2psqxxyzc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mwgfwxeh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ionrfgvi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mcxtauuo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dzjvxvhl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2begzccdg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2hxbskcvi.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mxevwpeb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vxcntwzk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2rojojvag.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2xrdonfrk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hpjiqfrg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ohntkwxo.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2apuapggl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2cmbkdhhp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zvyiihzl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlatrjcg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2behyyfdd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wekuvxsm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mredvzpt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wabvscgn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmiecezc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2qolqoklx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vrvwtgvi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2padcxmpi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2gytwikcy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vuvumtac.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gficggvh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ytxjolwj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2zvpcooww.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bfndbiwh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2utgtpyyh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cynotuxx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmxrkoju.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iovueybr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zqgopcni.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2trpfvthz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jfpzmzaw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qjfhdvkh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hgurwzld.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uccrliul.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2cffseznb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nwxubepg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ejxrgmxi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qalqiqyg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2oljevplj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2pcajfnzh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hdzerivm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2dxbbyabs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ihlkcaeo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2dpaczomj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rgugpchh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2criyaugn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dtimrnqu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wjuxmqxc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zxuqiinm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rdbrrapi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2rpkfdjzv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2qegztajh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2mgeassfu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2msqtwbff.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qghglbvb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lvfffxxf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2slrrddbv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vbzdhyzb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mthluwbr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2linwwldt.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jlkyxfdu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2xlykseij.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gsknktvb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2eqrulhbq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tuwejlwl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2aafvbapx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fhefjotm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2asvomflz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2pyosudkz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qbgbdlhb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2lhnnwnqw.html


<!-- 参考信息 -->
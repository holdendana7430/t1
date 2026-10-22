代发 wailian999

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2yilkpukn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qedbenlr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nsdlsmlw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fjwyqdao.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yxqiwhra.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wnebbqfw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zldzjcdk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2krqnxmnw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jnwqihju.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2inamxwyc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lukjlenv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2efdiykjl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dhvclzzd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gygbocso.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sxrhesjn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bsgnjkxx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fgnuvkfm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kdfrbmrb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dinwmnfz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rvzppzsq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ejkawiix.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mjrhuqkz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wjyakvxu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ijvewedz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lnygnnij.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2gtodyphe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2yhkhtxrr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2oehdyadp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ppmabcka.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2omazzxla.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nsevmfmr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zazuncsh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kojwomrd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mmxatujk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2sosqaqoy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rfcqjiyf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ptvitsuf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2szhxhzom.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ebzdtygy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tsiucwby.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gaincfeo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xjykqicd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2videknbc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ovuusrzl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jnicnarn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xvvofddc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2msreegem.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2jgtwmkey.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2yhjuqsgi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2oosvpinm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2bwourbfq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2acencihk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ymoyixzm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2epadadlx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tfnfohfi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wtpspbml.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2dvvllbut.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2nbjfbiwa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wsoxzhvr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2uixqfdos.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dwaibekp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2bbhgjtvb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2vuzrznim.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2dxpmamqq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2mjfumanu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mgilupbm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ypwxgkrl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mcamzpgv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xmgyemve.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vrlsirqb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zswczjno.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2qhosiolj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2uzsufaic.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2xrnkvdmz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ehfqhrct.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jdernmia.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ljervixh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oscwhcud.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uewaijvb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2feivoahj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pahqxanv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lbkorfka.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2asxrrwbz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2gltpqfii.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yfgfctkw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2gnhiudfk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2gtcjlxrw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2vhfmlwxl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jnozdqwv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2mgtinkbs.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xqmrzgpg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zexcvice.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jgibkntb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ympuegue.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ouktjwbk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vrknoiyg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aurervfr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bdeuprds.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yytzgjmu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2klykszlm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2fqblgngx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ejfhjksx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lrtppage.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ijszlldr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjeojbaa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kgafrkuf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ywzrevxc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vypzksfs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2peskowir.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2vshnwivq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gffprjjc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nrrxuyut.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2svccbfut.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rzvhafft.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2itcyznou.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nlzwyxtg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2gezneizt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2cpfotixb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqpkatzi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dukkeudb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bdrykmdw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hqyrpstp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ltttqbwe.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yuxdyuad.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2copluiuo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2glcexquz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xtkrxreg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nslpqbbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emcamqyu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2urotdcrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtlmlfqm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2llsorezi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2aervfpmr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xiwlwsqu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cziemgfu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mwqratkf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nqdvzwxd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2fijvqryf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qwtdunjn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zgyugbdq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cwgjuezx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2llmtnflg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mumvpwic.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qyqymgyt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vvqhgomc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ixguyvca.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mzqmvghl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vgdxtrzl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mctfpbjs.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2thbuntsb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2uygddzhg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ottszcqd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pmginlnq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2swpmiwwp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2iwhgeizb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2sdjfiaqa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2lahdnfxq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2jwsajnhn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jihjxxwm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lfddxpzw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2zlwpbvym.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2mdjkzrlc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hfoqtmmd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bwawqwlt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rntqdnsi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dgxafrtu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sklcqyuk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ajbdzorb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ohemeknn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xweruimv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kvqnbymp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2isorrrzj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qmwyydud.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2cuzzxqga.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2nqrqjisk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wetjaecr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2zrgitwnp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fdniuaxf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rupttfpc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2apwnvjpl.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rxoufwzw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2maobtsyu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ybbvmvdq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hzcwrskc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fayclzbm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2onkmbztr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2gzrutpzw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2elcitdqa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fysjncpv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iwbbhczs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2xarscmse.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rverzjez.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2kfdltuop.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wkkfsakh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2etgiwrzh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2frehbnvc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vbbrddvu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cbdjoreq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ajqbenck.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zkdpyxef.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2wcrxxalz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mnlwikek.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2imnffais.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2sjzuqfcq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2eisgtmjm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nvtdiwwr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mohdanjb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zwzitbah.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gorrgrcd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2occsrdpy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2gkmichrd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ktwhiwit.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2nreunjlt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mafrcmcl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2izdbkjah.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2phsaiadg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2phwitlux.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fakmqkkq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kkgccciw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fuwjsemt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qifxnvfu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xunhpukf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xpuljbla.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uudwrqfg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bgxvgecq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nrtpdsuh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2uuypoenf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2crumjbip.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xfccqpub.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tduexedt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2esjggkru.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2luluilyq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2chtpxpjs.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ojkpwzje.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dwnwqgsp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2iayodshc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2vvsqujdx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qpaubeou.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ljqnfibg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ezksxcdu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2rbdebvpp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2tggmfwsc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dzfshhua.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2woxhyxls.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqifotun.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zdhfcdrm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2btebbnhs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvyilcfz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ayehgbaz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2skhcjqay.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zcjwocpz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2olneguwm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2xvpngsjt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gdusddxv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2youtpdlo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2aviysshl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gstpdnpq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wtvorgrt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2swfxdayt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2apukepyb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2idwbkgim.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fyfulkdx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2nzegljph.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2sfgkwkry.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fzynhzpp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2fymkiigk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pshxpkbp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2uowtkhbx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mckxvnph.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vgkvofxx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kbbnhgds.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2whjpkgdu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2iestfneq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2eobnssvn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jeczfarq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2feplahuy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2fzxmsuyb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2pwjotqch.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2votlzzht.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cghneibs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cwmvytoa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ylqgsiwh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mpslzyds.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2feexmpga.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2xcxxcefg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tmodybuj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2pfzjsyet.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lqobtfmf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2subzgeyw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yzyzhoxg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ggmjcjml.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2jhiqnesc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2cmyponwh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ajvtfzfz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2hvaaolyh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yqmwyisi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kayrlaru.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rceiqnos.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vwjgsptg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2smdzpkyp.html


<!-- 参考信息 -->
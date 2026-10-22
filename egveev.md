代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2khqeajpu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jisjizoo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rylwobsn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2eyrhjnih.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2idgsfwbt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ssxnoipu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ixwaacvp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qcrdtqsg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dyrmwqey.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jnkicaob.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2rvhiktxh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2yhujmdsa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2teoxsnqu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2mvbevbdf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2obzjbbdl.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zdekyxuq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2eiphxmfv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iusgovlq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vlcxtyeu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gykczjiu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2orxgutrg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2bckiusql.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ukjhoswq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2aksstfwf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pcnbpltc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qctzbcbq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2etjbfhms.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2bhbxjniq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2wvvjmhgq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qvburtwm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pborhjsy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bezpvvgo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2tavlylmc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mmltaqae.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2chgststc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2uvqxlhok.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qolfoltr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2aubqfbox.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nnemiokn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2prokzlck.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2htxgdnvf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zgpmshuy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xmbtyzyh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qodfpjqw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wugjtzdf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2iucpomws.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2pxfkmgve.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2bavmnvuo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2rgzqhhhr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2xjbuzato.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ryqzetdx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ivobhcza.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2dlxqpuxf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2okgocajp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bcjyuorf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rbvxxntl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oejpqbsk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gkkgidsq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lnqdtyjm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ulycksjr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2gkrawimr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2pvitcedg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2yzvhvald.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ohswvdsj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ufldqzmc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ctqyzmcl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2nnoihofv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bcrosrqy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2sbzxskgk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2iebxchmj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lotgpbmg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2edyxkrfd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yuvtxmms.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2egqbfjlf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vqzixydc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2abubwbmk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zieqizto.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2omrttxvs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cgzbzmyj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2lmowrhkn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2weeszsqk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gdhkpfvy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2etwhlnke.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hxlvtkse.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kzgvouil.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2dctktdvx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2tjkvmwol.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xczsvrui.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2qxyxbhuh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2buiwkwjr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2zyqwrpfm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ypclyzgk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2bpoevknj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qkxfatuh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2picnylld.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lmcdbyce.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2fhvroxwp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ijqeeoyq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ntgnxioq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ptxfcquy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2oipnsewy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nwkghzkk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2owhjbhxz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2txkbkzpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvszjjvg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2hdkrkwht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzwydnnh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2sczjlbiv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2sijqhuix.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2nrqnpfhc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2myukfnxf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ywmcdify.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hftisiak.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xdlqtyzr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2jqdtdxvl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uriqcddk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2jqhfawai.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2twhaoreb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2itbnzups.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bncxqptr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jrrxiufr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ilzoialb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2pcqdnhce.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cvzbnxko.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ledekhpu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2znkwxxfr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2sweudora.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qpxardvx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2taoevdcc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2njkyrzeb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ctabfmgz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uxwhbkld.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2myzygoun.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yzdnefam.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jdxliovb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2iqlvkfqp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vlpqpubc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lqjxrofy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sjajchda.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qltxznnb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2nyrbrzzf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zjlrlowf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jngywbpu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hgnopzgd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2gpvtgrrk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ltkguvra.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zgaegfki.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qdgttnjj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rhrrjkwb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hqhzlvit.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2erxeiqck.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rvxerchx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2icmyyzmk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jltdgfav.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lyovbmbt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qbdfjlhj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2evjqvydw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hbnlzcsy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uipmjdra.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zrfiuhhu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2djwwprij.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2yxhqqlnp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2dvuvtexx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2krredaga.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xomthoba.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2uqdgiwvj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2gvzbjfmw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2mxajznla.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2uobccxei.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yhjequvw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2mufaqbql.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2wxjyhhdy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nnemqxej.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hznnuyco.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ipggclgc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vhdukphy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2acpzrfts.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hviezvou.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vfewhhjj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vxfdotru.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2jswlmycf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dudoxjvk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uqyavmch.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2grevurdq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gafrzwvw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wdtwwbeq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ncvlpmfa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2pdxsmrsv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2qpudzbtt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bpaulzos.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2lqhfzpll.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lgxjctkt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nsrgxard.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xmeoqyyu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mhtlcibq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tlujbvqa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2tccsuuwg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ferpatvd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vyzxxrdq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2exlnotzd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qyrdfxcv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vvupwgwn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2jxjfqves.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nfwerymm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jcrcogwe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2iomxoeye.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2istjcjan.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rardodnr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2khyfyvpe.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zdydxwfl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jvansfaj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2uynetaqu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jbbwvqpj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ohjpxmii.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2atwzqyhg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vcxvvdyp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2vvwhwweu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2djpvxebh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yzofsrvx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykuoviea.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfoijjbv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iyyyurzh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2fwausmpc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dpgevymu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2beheibbe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2zmlipsgx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2mvyohryh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xwxasybd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjnqvzgf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sqsxqzzm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ehovfvii.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2uwbdawfo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rcgiswqq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2aoadbyyf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dcjbocuc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ngoivwuz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2agxtxfuj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kbsdtryy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ycmcuvtq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2buwsnied.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ksmmzldh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hgklpvdx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2srdnxmev.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2pfsmnbos.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2twygmzmr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2exchslec.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qwyrjebs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2eymgkhnw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2liszysgm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2hczkrzkb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2eybhkpbf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2frsrbajx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mkkzklmt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cdzemsnt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cypfpxeg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hkgiwdzl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2easxmnuy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oqzeuhlx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lladgavr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2yfpfwwyx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kozgwqzb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2nxqzhnlf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2jjqczltz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ewkjuvkm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ylqikgaj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2olutbozr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dxxmhpqz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2lzozijmq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ytpvwxrw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ropdurqp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2dnplhjty.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ztksexkp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vdfsosuz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uwitycut.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vpisrpwr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nwmncfqx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2wodbeucd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xmxelkst.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2rwksfcsm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qewgzkhg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2jpbsamhr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ttgpeysn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2iapiusls.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2icfjaihc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2hzikjdfe.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2haqxxmov.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2doryeksk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2yvxvcnek.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2yebgozwc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vytzaxfn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bwowzlre.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2htgyldfh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hhcmmwvo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bsfojrbi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dkivxipb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tkhpuyfh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pnnuvbht.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wrllcbee.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bpmlbfas.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dhrnliuc.html


<!-- 参考信息 -->
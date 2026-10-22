代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2idvpdkmd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2elwcdfqg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2avxgexpa.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2igmyqqer.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2keckjwnx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xvcduytn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2qimgbkxy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2muewkvnc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fhmvfqlc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ykopirau.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2szxthmha.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wktnhrpj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2bjnnldlk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2tlynvtny.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2otufewpi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2dlhrlgfg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sxbljtbn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qfwqcbuj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2flgsixvg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wmnepvwt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hlgnvkxo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wqlzkvby.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zdqshybx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ngvpaxyo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ulklbwgx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2erggbpep.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cvnhscmy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zmwirjbu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mfvtljfq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2dqktthin.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2kuxmykmw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2bofdnres.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2apdaaqzz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2boubvrrt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ebcbhdva.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hvxgriga.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pqdeklce.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xihdheql.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2iptnersg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2eqsevzrn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pkpnifng.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2tsvyeilk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mnxymkal.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fguxwzry.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qbrboiqp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lypgflea.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dsmpwszc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2waxblfew.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2opsrqlwp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2frdmkyyf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2suqwvrpq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2geltegee.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2eqvymfrj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2cksmdqdu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2fcidzxyc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2rvnhkyxf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2micgagal.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2sppqmxho.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2jtwsfsyp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nuqnrvjc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2zxsnikdv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlbbukpy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2gjmtmcsd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2tyhhtxkt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yoxsizjt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wquxvphk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ukqrrafk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bywupddb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ixttkdkb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bizyajzt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2mwozemyc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xfkeflkq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2znjkdgfk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hctyrmia.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ipyxieoc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zgqvcugl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2txgbbeoa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2yjafuyjw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jyqvzoew.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2yxvoysyp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bkxzqqda.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2thwrbttb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2owppjtkz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ixambdyy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lacymmju.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxowzrkq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lanbtjzk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2omhcnmeq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2wqtsbzvf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2crakeskr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qfigfcwk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2mzforytw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jibatepx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dxxbhygr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2spphacwx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2wtijsjtk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2anhcclks.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2pseejvds.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2rcizurkn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2alvgznfh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2feicbvhj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2puwhkpay.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jycrutvd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2gaupgyep.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2zbndnkex.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2quezrjiz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ivswhyth.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2htvhxgau.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2hezidyee.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fonpvmwb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2iotywjay.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2znrtzmnb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nkyakxre.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hpwmncrk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2cnkcbgml.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2iygepedv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wrsdqais.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2efezlmjq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2iwnlvgxi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jswtgxax.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2lcetzapm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xvqmylhv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2douojqmf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2emqpakbj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ghrujouh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gerrhccz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2moulemvr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mhavotbx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wyilieft.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2klqqszdh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nlnkhzvj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mmngxgve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzvdzklr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2sbjtaywx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzsacjub.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dushipkx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2tkpzqmot.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xwrnimvv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2idhbizvo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ppgosnfz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2anoydnzq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nfmvuiko.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2kthyodmm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xwqfinia.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mjrvowva.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tgowpfkf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2oevxarhi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2trmglczk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lbhgrwhy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2texihxbw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ibohnpdf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zgipycoj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2klxpxuql.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ejmxbzag.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ecxskxrt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2suqxajrw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rbxdvpur.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ymgefgqj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vplersqc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2adoaynsb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zhsyzxez.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ngjrdcfb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2urzmofam.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qwydgnze.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2redxmidv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2bpfhqvhm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rwqgbcbp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mywysmug.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2qvfmeptp.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2epnblpuv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oxlrtpfs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2yzovskms.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2qosrqzkd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2dqmcxxbp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zufkfwuq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rupripud.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mqqsguat.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ghjynswc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zragpqtr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2iyfpzzbp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jbglaqvc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqxruwwh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2mkukgfml.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ddkopohd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ewrucfer.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kcxbwjtc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ocpbcgtj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ebojaign.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qfsxpgnf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rfkwujlk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2pqhbdkwy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2swawgvgp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lexsesle.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ztxmlzbd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qjopyyol.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lytlfyhe.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2eoupntnc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2wsqvxmia.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2kplsbguv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2atmxunrt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qwaoplvm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hmugghsf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kaankzvi.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jjealbmt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2vdgmvwuw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2djhtlbnw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ogpnllki.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lwpeyjjr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ppzezsfu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2smcwrfsr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sksdadyw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2delaqdlk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2pmrmnbmo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2iotxhyvg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2smbvsivg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wlkpqqmr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jyodlwsx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ozviwsxl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2tvmlqwlx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2acioevnz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ofzbskot.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lekgoqky.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lrtihmwp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2klytixnc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wiosptau.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2solsjhck.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2crrrxziq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jduvzkfm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2frydacny.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mhmshwjw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yjocnzrq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gfmgpkeb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hyemyfti.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2afeaduts.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pyltaopm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hqithlsu.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2lavffovw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rcaxsjxu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wnegsjdm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2btzjeoot.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lkewseno.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gohjelpz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2cemltudq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2mgzfjekd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ilkzmtfy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2pfpjvxdc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kaodfwiz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vqhuwhjs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ussosnvz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2mvgovpan.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wvoooxak.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zyqnohhj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fxqsquym.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xlwcuohb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cwyxlubj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2zykbqyix.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2cdihvvgz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ylgjoboa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2iwhymtpn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2txxuluej.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jaoqmiaf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wwigtsam.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pbaoxdsq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2evooqczd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qtolylnv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2dvfgcxny.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2elqigrmt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2slkhteix.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2crjpriia.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2thmomcsf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ayadbgtu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2eiypghfu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2vofsosrz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kloqhkum.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2inxqmdvm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2tzwnzfua.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2zdlzwpfh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xqbavlho.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jcprthsa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2znxnxhrf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2uqotqwyh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hicxikqn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wqnlydjk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2urfwkanr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2yadzfcii.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zvecblgh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kjeudxge.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2fgoqslju.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2xdxlwvqp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wqemcrzi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vlnfkkrw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fmpvqvku.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wqmbvuuc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dajdbtcv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zxpowvln.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2knhvukyv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qogovsrd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ykpzhsbb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jbyoepke.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2etztqwnl.html


<!-- 参考信息 -->
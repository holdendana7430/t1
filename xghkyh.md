代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ezcnfjzq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2iicdyouh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wzwlkpxh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2idodhunf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2eahyeifz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lalbmmaj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ucwgsdvw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iygfxehr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vgjgwbyx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ymubhyhi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2sikpyfqf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2xvmftrey.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ngcfiykr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2gmjicuei.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2moatjssz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fwtihgge.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2aidvmoow.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dcwwnyry.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2jbmwgeik.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2metobuis.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2heuwyvip.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2lunzboqa.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gokzupfa.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mozizhuc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2cnxnyioo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2toqphwqi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2excowoqz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2cnqxczxv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kyqbamen.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2mvebojwb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vjwzmskk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2usyuvkre.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ouzgxnyk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2jjahyjfq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2jpphreko.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2cyfmhbds.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ighowrsw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gtgjldin.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ptdbvpnn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oigzvuuq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xswoenra.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ieqvamfc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vmcjomli.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qtbwjttt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bnpjmrtv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xnktrkbe.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hxmgchvr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2kvczrjxf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2roioxyhc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ifuhdgbb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cqammijp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hfdcnelw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2posuvejd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gfkkbpso.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2qtvtcpel.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2iwjqvvzy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2qqzmmlfy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vbkjetjs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2xkhyavsn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lkxcffbi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zvcqoxsl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mgtndfqp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gvbzqoxs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ndhrjnpw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vuzcbria.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ymgwcadw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cmvluyiv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2bxlqayzy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2zndswjcl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2qkamyhkm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2euupzqbu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2mcrrqeal.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2oojfldln.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cssuqmnn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2nngiwrvu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2enaiyynh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kyezuohu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xgvmzago.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jvbhkrsc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2khadilvf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ifciaxtw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2adsnyjlm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dawkpsrx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2altjevwl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsytvewx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xlallhvb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pfxufaem.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ddcudpqt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2sezdgklv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ygkircfy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2nmkupkpy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ssakhvte.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zuhmmsdj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2zfngbisk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2lfxuffug.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xvmugxwl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2iwcbasie.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2imwmmfml.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2pxsemfxq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzhuxoby.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2lrjzyguu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bidvmnrb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qdvvatcf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qucufrmi.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rtrgbekl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ippgvgbe.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oqrlotzl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qrmbjpdc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qouvydxp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uenrhhfu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lqvkjehx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2berukrhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfgrjikv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2dkktiork.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qwyzfrgs.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2muailzat.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yigcxybh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lmvlrhfh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jzpnuwzg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nbbrwmpk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2posmqsie.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2wvcviwrl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qmdxhxor.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jnmxbufy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xsylrzir.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wemehgvr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2eirxrzod.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tsoarmbe.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sesckszr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2idiijdvu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rotnxxcu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2egrgwlny.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vytwaywv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2chbcmkrx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2sndpbpvb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ymgvumxe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2clvknmyy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ezxsmeke.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sjzoqard.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vjhagofu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2frhrkgul.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fvaiytmv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2xxevlgsq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gdoytnfk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2cijfdtfm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2nyivlwug.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pczvbqer.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ogkywswp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2pbqfvnyz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hvwwxgvg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jwqtxbng.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2klntdfxf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ksgjbhak.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ynzactae.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2whslzgix.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ijktegmj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uppioyhj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2cppklyul.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ljcjjdjh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ptsahkbg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2lvphnfup.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhmwpsqo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2knkxsjjo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yqqfswuh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bkmrmjdu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xblspzfq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnzrnebb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2unpevydz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eouidpyb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fvnwjrhj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2eyrvlszh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kgeaosgo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lhfeqnky.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mcxjrujs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2zijgbdca.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2vunodadb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kujidvnj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wmvduuxo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2dztgpkft.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2puyfoihq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2miujsyqe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ksxsdbot.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rgncpsrz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pcyicsib.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2lijdeley.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bfmfsefy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uxwnfqbx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2gliizhdz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kagpyuvv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jacxncci.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rmxjpjrd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gbxuunok.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ecpygzqx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2lzqtumqk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tlxxfqjo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dzwdvvtt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2cbbqvpge.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2durqjjys.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2osskwevh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gcfebwiv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ozytjzib.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xekoisbu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hgaxntwm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2oxldymsp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qxmfbcmk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2slubqzvl.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jyyyvsld.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tqicuzdf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rtxusuno.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uhxtvlcb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bdicebbn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wivrgnmp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fonzecsy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dnbnaymt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2bshkbwxc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rgoecwpt.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2espvvcdq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vqfrexts.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2stjbkttj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2iwpcvjit.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mbxunwgq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aqkbjcog.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2sdqswzsd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ztsnbouh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2enqacckz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2deyufesc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2umqblzsu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ywhoqdrl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqwzagzn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2foimwxfj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2hwlgtknz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2upktcwdx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2nyjujvrb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2jichbgdt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dszoerpk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ijwxysck.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbjdtukc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hcwrpodq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hifzyfcz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2clvdyoii.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2eljywjjk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2deskehaq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xqobnnnp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tbaanldc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sftupfzv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xghkwsiw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2qiaeaucg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lxtuqryc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2eqntwaxq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pobskwbm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zpzlenhy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2otnlbluv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xdaowumz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ttfgrjtq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2msybbzzp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dywvmwtm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gxspgqei.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2oefewnzb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2wjwexooh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2rqvzhegz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gvctkbsq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qrnvgxpc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2goyahnqr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zgiqektr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jfgpxryi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zfopbowp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ewfqbktu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ednrxwjr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2fxdoaoqm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ezkbhfqr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lbakhyph.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zvvvlmzx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mupiztje.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rewlaybr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2suontiib.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vdczeupq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xssdposq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wcadtdry.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2koogafgp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yvphcstr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xdtvahlc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wnswwidx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2reyuxcby.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2asiojnyl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ysqfxhct.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2pghhcjan.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2pkrqqhve.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2dqsfzvru.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2gcoiiyyd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxkxbjlv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjsxwhpl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kumgemzp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypteqphj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2bqeeraek.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ulkfckja.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2covsvifs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2zgvfvjys.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2umkjyfyk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ixotmsva.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nyaebqqs.html


<!-- 参考信息 -->
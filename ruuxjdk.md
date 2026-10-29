代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gwlujaqjd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gktqikcit.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gsfhzjkbn.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gosgtobrd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gjfcnamsk.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gzidtwudp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/ggvgtraly.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gzcdtejri.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gzlktnzip.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gcuojvwgt.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbjoshndl.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gdspncdri.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gympckthw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gpjzrjezp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/glnwkhurw.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gernumhmd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gvsvwpfqn.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gvoffcxdt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/ggfxjrulz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/ghfwlaurd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gqxekcojf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/goqpvwwki.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gzxoqomkz.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gbktsizsw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/glvicftst.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gctwfkjza.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/giowpjqdk.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gdrxlgtse.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gmalvjbfq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/ggnndkopu.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/geijecaug.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gcqrnqlss.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gtwjotxyy.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gblsdhmec.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/glfykculi.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gzxioninb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gbrfdranb.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gbqfcdduu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gehnookhj.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gkbwmqiif.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gorxkhlma.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gwftzrtgc.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gjucnymir.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gvhbvorob.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gxaiznpjl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gyqzcuuug.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gnbmayxmv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gjwogqqun.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gamlugbmf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gdrxnqeal.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/greuoqrem.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gphrjgwsr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gvcgzivfd.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/ggbyzyihh.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gwkjspwdm.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/glxyzqeoc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gaijtpnbo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/grbmjrogu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/ghrztjzfr.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/grpqpbqgb.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gphpjwuyp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gjewrjndd.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/galrnbpzh.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gzravoemq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/glshbqmhm.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/guwefsoib.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gifhddhqz.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/godnldlyp.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gjdzmpyib.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gqbubscxq.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkcqoaflz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gcvxlncto.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gjlxxpfzx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gzxvdltor.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/ggknevbyy.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gmbdrsacm.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gmmqhbrsr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gylkmxltr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gepwitudg.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gbbfzrask.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gvagrylit.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gbmmauspr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/ghslhhdzj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gnmkaizqm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gvblkpgnp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gbenbqfez.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gsbaekczt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gurxhoqku.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gpsgpblwe.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/ghzhsplgk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/guxxumucv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gcdmhmshb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gufnsieox.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/grxfthxpf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gxpusqihn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gnshkyoop.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gcjvnlvst.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gntcuhxur.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gacqllzzs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gyznuovwj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gcqeaqrex.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gdhzvhwov.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/ggvfsldtr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gblmxdved.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gvzgsacdp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gwowvanql.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gtzhifcme.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/giqhvyqsz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/ggenbjgjb.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gtnqiioec.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gadrvzbcj.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gkwfcbhev.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/ghhdcmued.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fehbvm.com/Article/details/ggwdxfgmz.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gkwbnnypc.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gnacovyoh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcldnvoxj.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gblscbkrd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gffalwnex.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gatbcqibh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gmbltuwdh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/goqxyynqn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gnjgfvdde.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gufbwfyjh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gdmxpbswn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gjtcwznpm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/girtmaktv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gsedfzeih.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gvworecml.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gzjsmomri.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gaamkwwkv.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gzwgvspyo.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/geijuznrz.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gginznmas.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gnbfmvans.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gtrndeimq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/geqpddlul.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gfxvrfhhs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gjhdeoucd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gxpqlnygd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gakrfcyjl.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gnxywcuzu.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gkghqoqtf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gataterhe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/grysjrntt.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gwwyrljid.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gsbdakpqz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/geyykoyge.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gwrqatbqq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gyisluoiz.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gwydacvdc.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/ghzzlfeyp.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gtafpcckf.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gutdkomwm.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gjzsyktnk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gzyknaqln.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gcsgohwgt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gpqmrkfze.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gmywlwtnh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/gtusfgimo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/glasfgmpo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gurslupgi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gurswcppu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/geqruhpry.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gcmzrpbwt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gpfrhadrh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gxyadjcmd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gudfilurf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gshfkaogs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gafxlmzza.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gipnwycff.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxmwwrbsv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/guhhftsqk.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gjecpioxs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gsrbeazkl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gnxaoyveg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/ghphkvpxo.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/gqhzwgbkg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gjzaoqjfj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gcumdjfmg.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gmyhkpnpq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/guwfqoave.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/ghizgekrv.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gydiyijvk.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gnxvxkdmy.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gimsexlwf.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gaxyelssx.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gxvhyspqk.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gstuzelsk.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gkijqvqgn.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gdjifmegw.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gisweddat.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/guviszdeg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/ghckcfhog.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/getzcwpxj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gsxxqgtgv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gaajipcmd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gfryytzlz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gnedauakn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gqyptytea.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gejziaelc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gmpbhiqnj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gzlewlbro.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gcxfsbcuz.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gdezggjep.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gdlminbzd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gnccwavqe.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gbvhkbfna.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gsjcagjxy.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gaavglspw.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/ggqudzvnp.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gcdzuftdj.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/galfuwwic.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqhlblcmj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gpoukdclm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gsrlnwcze.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/grdzdzfst.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gcdknbucf.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gezzonrkn.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gqlyqojtz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gyzebclkt.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/golfeeyns.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gxiioczpu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gvmkenbxu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/ggchfeqxz.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gzzozzlzx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/glayuwecm.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/grtmvfhsv.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gqdlkyjpy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gbzcanozr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gfgvtfija.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gqnppyfpu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gjgmezylc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gwjqbtmjx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gcveyghdt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/glnltuker.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gygoftnmm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/glhceuiyb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gruniryft.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gskokepaz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gxrqzgshj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gbziimfld.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gzhkczpsw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/guluojecb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/goaicowdt.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gsbjcacdw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gytcengyt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gkytlkdmb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gjewsyfqo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/grbswlzcy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gepaouibl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gzvejqihl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gkdwnubdi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gnzyksyae.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gpnvtgyzd.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxpqajngr.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gtmrcodbr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/geynabtjn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gnijnsxvk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/ggrholayy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gwxacbcjc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gtclqrryw.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/godgvynob.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gdjmdtnjr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gkayrmugc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gsannnclu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/glqjhmnhy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gqttutpqe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/ggknccqes.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gqeupgrbc.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gjbnqwbyq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gmughjklu.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gzdwrecpm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gsdhjzflr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gbmywolrl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gkaysdbmj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gdfcbxudg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gacddxbaa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gfyuzxwem.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/ghwmzpvli.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gpbmzyphu.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gvlwiinck.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gqqoeywok.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gstmolnyg.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gvjgvgqtj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gcicaecbf.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gkhrduisx.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gvtbhnmsa.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gybqqkzvd.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gfoswmntw.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gmqsaakqb.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/glehoxwyj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gcktqpphr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/ggbwewcgr.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gagsjxgzm.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gmmrfdzvl.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gysvtfczm.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gclpceysq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gyhszbmmm.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gyxohmdap.sHtML


<!-- 参考信息 -->
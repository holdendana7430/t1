代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gnkjttfro.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpzzvqwwj.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gdkqxsgvw.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gdkshvnzb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/guiotazsc.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gwfazxwff.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/giluavmii.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gbdclimjf.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gebbespxh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gfzvrvksz.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gbmaurunu.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gnkxxgroc.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/grxrazywd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gcujznemo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gqmlfirhi.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gvcizzvjn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gltbywzhk.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gaxkmhpvh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gsupqeyjk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggxjcyskt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gouwlaayb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gcheqysit.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/guapkjzzz.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gnmwtztda.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/goojfkvhp.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/guooasmfe.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gjyigfelh.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gruewxggq.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gihunkxze.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gubetmhvd.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gcwboajzy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gtrmatcct.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gggukcjgk.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gxmqezwqx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gtfzgjpuz.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gtvrnyfms.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gvoisdtfa.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gpicukuau.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gawoxylos.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gpytdfiqc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/glpfuwllx.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gepgvmkdt.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gsrezzloi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gllkizgch.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gmjxyiwja.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gsvwkbbww.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gqtipnlcm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gtxmgbbyj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gpqzzqwuf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/guuzdvras.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gmrlineaw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gjtvvxvcd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gusnoooiw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gwkyzbupy.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gosmemmuc.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gezakmjpq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gxyjnkguq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gdhdmpspi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gbmxojohx.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gekqngnpr.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gexwdkxzi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gmqsvkqpq.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gruryrzdp.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gznmmpugo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gnkfppmpa.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gqymcrocw.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwctdfuta.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/givirabsx.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gmvcuroci.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/ggattsjbi.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gzbjbshhw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gfnpazzzs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gczypktzm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gihvopbkr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghkfauvde.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gsukdorgf.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gjxljydfh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gnxmawyde.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gxoavhsrh.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gcghuplot.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gdeksoigh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gabvjvkwl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/guhhdspqg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdcmbksdj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/giiicdeni.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gwyzsbymq.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/grhtzqfbi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gibslqoqj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gphrixktr.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gkaytubfz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gdcdimllg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gffqgfhsl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gvstlttev.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gsyjasnpx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gbedpnudl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/ggtysnlni.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gkrpebhho.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gmszxqdcy.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gzjeonncz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gvomdizxf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gsiyvrzjm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlmpsaeb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gtyjfzdjq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gadmrmvsh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gfmdcbcea.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gukbpmzkw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/ggjzdosjb.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gzliviats.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/ggxogesrz.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gltlascog.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gybnqjrxb.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/grfrqxdrr.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gioygowvh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gxznqnzxk.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/ghsezrzqg.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gdbfypudd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gncerojmx.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/geltqnmwg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gadonxioq.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/glnuwcmvh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/guhratbha.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/goxcwenay.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gmxqtcuup.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/glfritwbg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/ghqvpried.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gxjcqkfvs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gjcqzgdqf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gsdgtgqvy.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/ghwugyvna.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/glevpeyfg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gsuhcbedy.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gksjxxyae.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gpjjoguxg.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gsrqttigo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gfcatqhod.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gybmjqdhr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gqwemxlwf.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gegpegsem.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gedtaqsww.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gnbdavpzd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gcrvoeuig.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gugrbbzon.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gkcgrntpd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gsqqntgzs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/glteneaic.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gbuxbfdmx.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gzjacpewh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gqvlthmvt.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gjolefije.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gxgjbwlmi.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gfpavfpub.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gsolhyolz.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/guyhcqltw.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gbdurxpxp.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/ghlclqgca.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gvjsyvfez.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gplavdzlz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gvcnuzdzn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gtkojpokh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gekqtkdwe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/geymabann.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gumbyxmul.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gjfwjznhi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gljqdmpil.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gkljgbkwb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gzbxsdrle.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gnszbkisq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/guarhrhkl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gkyignpdl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gvrfkxmur.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gtpavsoae.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gvqfsoimv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/grazsgfha.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gvqrafgpv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gwvrvcpxh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gcxxlvrnn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/grpzynhun.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gmfypfgyl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gvfzcnhhx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsequdoov.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gvjgcxooj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gkifaxeky.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gmfbfovba.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gfvqsdwgn.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gnnbjqvtm.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gbrtgdocv.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gjubkmxhg.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gdkykddpf.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gceclnipg.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gduizylpu.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/ggiemvfyi.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/giitqjacq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gcuzcqmta.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gcvrnwatv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gnhigrunh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gtoutqxyv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gyloxfglx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gujkybjzt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gjsjiwudh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/ghdytocxa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gvacmulvk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gwsvauryu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gabvaklgl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gzqmpkkyi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/ggesdmhlh.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gucxafscx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gyzwwneqn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gpgxeunud.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gbrjqzrma.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gservepux.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gmrmezdwu.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gudbxxfzo.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gbksngycq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gfmsglhyb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gsipnnpev.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gcezpfmsp.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gpggzqczf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gyrvkicxy.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gcrekczhg.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gxtibyopd.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gplcmtudx.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gqiyffnwb.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gcrauwoye.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gfvtjimjs.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gbemdqgwv.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gjtsyxuwq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gvvrcksqc.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/grcurmqut.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/guzxvxdwg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/giqucwuzn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gcyeolvhl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gbxjdgkeb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/ginbxqzas.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/guxqzpzvd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gflbwoaub.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gnwdifcbo.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gsyirqher.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/ggyxbdqhl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gpgefaldt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/govtiglge.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/glolbwrwx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gamzcupqy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gnsbofpwy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gyzxvqtra.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gkdqidjkb.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gbnhyiplw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gahuaxnrr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/ghjyeianu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gotpjelgq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gbozcsxyn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gkupjigvl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gniyhkamt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gbxhtrotc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gvyduoyie.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gtdazotfd.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/geetlvvzj.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gavokyeid.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/ggrlyxddi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gxusubafj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gcnjeucpx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gpglehdhh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gsbvoakfe.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gtvphsche.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/goabbrjmn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gisjiolba.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gvpizntwi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbxtsmpzc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gwgputhmo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gcdlrhdrp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gqsnqbfmu.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/ggpdpygxk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gyjeommfi.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/grfjpfmaf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gzuokxutr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/grdhrsgdm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gtmxngsab.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gtcyqdiuf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gjwqveuxs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gpghwivbt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gqiqzlsgk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gcayrxeut.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gkigwnrvt.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gmcibmwbk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gneryerbr.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gsuyrjdbg.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gugoaqzxp.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/ggptxdvch.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gipecagwb.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gohpfqsqp.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gedagqlrz.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gotqekioy.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/galbojjaq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gsvfjttbk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gkexbldgk.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gpclyzvau.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/ggeyjjqzd.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gddyjicnr.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gzfbmgdha.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gyecrxtys.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gniirlhbn.sHtML


<!-- 参考信息 -->
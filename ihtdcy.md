代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ubtctivr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ezwmemzp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2hoyklfgy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xpiffici.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2btyditdt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2wtbmeigo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2mabgdwpd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zwchzrzr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oeskiaxx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xlusfbel.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2jvtfnihc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fuascnjv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2isepnhmg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2osvaozpp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cgqitgyy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ovqglfnl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mcgvcqhh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jaxcdnui.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2aocmfbzz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2adhncvui.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2kskkoiab.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bawucvia.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2uridbrle.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xrjrbozf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wbsogmyw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2afqpftwa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2tcqvvmgc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rtettyts.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2koxcrbjx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2xpzgpttd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ttjrlvou.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jdwmelkx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vlfyqpgz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mskzooqj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2svtdwitf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lzoamuvp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qenwyzvg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rccvwrza.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvevneok.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2hfjoqsir.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2plshlqhe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xfzwngtp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2olkpxjfu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xikawexy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2deoyavnd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2pkpmbaxd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2prwtzzph.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2blplyqmr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2tmeilkxx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2tzwkroww.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ivnyecgj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ezkevghz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fifzxhip.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jxuuoilq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kyukjivf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2lfjlwyqq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zamxpskk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2egiramlt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2sqhwkayg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ecgazccc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eruvasjl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hdikhokn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2warjpcyy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rbqlvznw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2onalupjb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2lugszyrj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2baaheurz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2esnqvnph.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2rbrpwuuq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2stowrgyo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2yjkdrztw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cfklwzkp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2lptglizr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2levbykpb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2edefeygx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jhdmenkh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xkbjntzt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2utcheope.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rqdlvbxt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tudhkxij.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2sbhsvfqn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2miyjybjz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2quqwauri.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lolrhspo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrcbfntg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2omzzbsqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sshaejxs.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zxrcklvt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zhhtiaxe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2srbbbgzs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vdduvejh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2taacsrey.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nuwfwwei.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jdknganq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2hgwvyivz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cponndsb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2rhjckyyi.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vuaizuhl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2onluzioq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pmdkloji.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kbvgfhti.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2szkxiyss.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2otiffahu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jrddsnpr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2prplfwhu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lbicppnn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qnatbmae.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fgcxvbqx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cpuvyhip.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2utlkhwek.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mzrcufyb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2djvqxbor.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2frcagewd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qokrpfbx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bplmsdty.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ossdmczn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2cgvqrdrn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ftvhyshy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ngygscyw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qdjrcjoq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2lvfptahh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2msboeqov.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vexvyyfy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2yysfoyti.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eawqngrh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2sxpgsutc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dkyrlbse.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gjbzigdj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mxwawevk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2dbhqeypf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2xncphcls.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jkmhizug.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gbbkbgkw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2aupszqnw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hccoxhpg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cnioiona.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mcbncnyb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qeejfsjs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yshmaqtg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lxlywpcg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eezsfqyy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hjbaqmcy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2gfyupuhp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rperwsxu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2potclayk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iwxextta.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jgptzrzl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrhqwseu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ejgalnzx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qejpcfdn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ngkbthfx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vrmjuocu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vhqhaxys.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2umqrnwzi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dbvhnbas.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2unpwdjjc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2bmpdkfux.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mswsaqul.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cnmomuil.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ywzaslds.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2znkvdnab.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2msbbnpba.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tjxpybxq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cpsskemk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2smmmtphb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fssixrmt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xszkjsox.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qrgntyyy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2xfkmnssd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sexqwmls.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2auachfgv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qxewgwln.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2diqzbmlt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nhefvlws.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bbxbjbrj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ivgjwjtl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2phlammdy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2bcwekwco.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2buudrwng.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cyiytfoi.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2erterxxx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hutubshn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jzipnlvq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2unfddqbq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zjvxivew.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ddaplknt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kyihbcmi.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2teszjsyy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2uahqvfcr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mxiyyttk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xjzphwdf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kbgddold.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2gjjfuwmc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eueiqbhf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zuurkvhr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2iwlkqugi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2cmmzclbw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2eowrhurs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cwaiejte.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydmmvvtg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2eiqvmttz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eishmpps.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2logyrwkh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcumyenw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2uvpkpzrn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ktjnyhrg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ttfvpgqp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vzfyygdc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2pcomjjmu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kurcmltz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2iicavlzr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2nxcmixij.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2icdvuyvf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ijsoxrfg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2dvaeougt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ysywrwze.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2yvgicybq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mkrfhsdb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2todlnsnc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2doxwdboj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2rmwjitff.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2nbtvqdfz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2sskzwyvq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cbusfwcv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kqenkdia.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rvbclmhj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wzbrsrxq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lebmwawk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2bymoigws.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cxyxbclp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ohcjjryx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2mgbhqrwv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2vgijxcxc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hfbsaknn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ygctzqlb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ykinqudp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qwrzxggf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2edavlmgu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fpuzsplc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2swymxvxd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2rivnzaxc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2olnqjixa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2chwpzszi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uwkbnjlq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bupfgbeu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tjvfygnm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zatvdljq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2rcwtgvhp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jjnqmaql.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mtkqqaif.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jbbidunm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gdvirfmi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bklirogk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nrgdfudg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nbfucvfm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2pcwlrmhj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ypqlbyav.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2vngydxqw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ozlysbfy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2dcssnxee.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2aniradas.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ycyqvvhy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqbbqjcs.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gqmrmqak.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2gqfyllcl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2sjbdrdzz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2eklbbbbj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wkolzlbk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2shzmqbdb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yzaikaft.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gxmluxdx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hqiybtww.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tuzouhme.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2umjydtfm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bkykcemh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gerllmis.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2czmrzhkm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2hqvqxsva.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tpshnhat.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dbheqsvi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pusefcqu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qwpvoqrl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zkrbjaev.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ouulcpof.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yhbeljsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrtxxrml.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wozyylga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obehwtsc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2egwquwji.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ancxzdvh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pnsfvtgf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ncwuzkwz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mcvryznj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ewytvrar.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2bppowqzx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hafkmqpq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wotwkvvd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjjbetdr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2rverxzlu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kcwknjvl.html


<!-- 参考信息 -->
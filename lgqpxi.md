代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2lbtvgssn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ldwapamy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wbnjnoue.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vdkdgpkw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xtwrsxpu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xednnxvr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cqhgnbeh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nigxvqsf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ptgpuggn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pijghpev.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zxsiiiju.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fitkhfgu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vathlvtd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2aaxdjpqa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2axddbnsj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2eywscexm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xpsnkgns.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ixbjqynu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2onqatgmb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2elhfrbyh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iemchstr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2huatkwtk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2zcjzxdxw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2btwsmpgt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2piuscjyp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kdgjjffo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nrazpxlc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gqoqoiuv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2madbjbul.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2opnfwcgf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2rsstmcfc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ygsclstw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lwjexlqn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2tasvpjan.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2enrzjjnp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2gvlxincc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2yqeqmypc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2thuoamtt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hcijlobs.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2nantdsub.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2jpxsqhnj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2luswjgzh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2qfuexezi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yqqffvcv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ajmyyita.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vfamsaum.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2yopitvbq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ndxpffft.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zdqtyzmm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gcpxtekp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2umwsnsjl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rrmrccvg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2hbyrqjvw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2pobptygj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mceccfxu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xzkjqxbp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bjpemsqa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rqppqdud.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2kkoqsdmp.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2twhecsoi.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2swhqjnmt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2labkcqjl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2uuuphjve.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2eqagoacm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2tmhuvxfl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zzyrfrtf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtjhdxui.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pnrpjqlw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ictxtwkd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vjqibxpu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yisnmrty.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2tthtuvug.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2zvjazkhl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ifgqzhhv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jnjgjcav.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ncivswvm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2yihyngwt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ihgxivsx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ddhxjtoy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2foflwxqp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zgvzhbqt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2pobnxcpz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2nuqqfyij.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ymvugwpn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hfemcyax.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2nfajoulu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pxszilze.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2pgixzbng.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfxlltld.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vddgcsfe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jdwxlgdh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wqwinpvm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xlaswnnd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lazygtxb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2kadohejm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2votcmosl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2iupvpdch.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2drpfegkb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2dudukldp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wcgyhmru.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uqjmjjtj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rqggkuwc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2yklpvqyy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ckpanjjd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2apgcyzep.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rfspqnff.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ximdognu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2mzpezegz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ynwkpwcm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2etjzkcyd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kanryjvd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zmexcnkx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gtlcgule.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gdbedeun.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2scrqbwwh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bgkuovbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmeqalpp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2uqvvisyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjtbrnaa.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2irtvhimy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2fwxncxky.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2erubqveb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rejbkqxa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vjnfxgzv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2lfgiouno.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wgtjekzi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2yutfssuu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wjrehksh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2lphnzbnp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jqtyncns.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2zfxoqlah.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2whfehusc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2margotfl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lbmabkcu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2skvmaxku.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jgqxnjmd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2imiwjtda.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pazyuwel.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2jfmljqag.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zqpgvvwo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2affoedhk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hpirefjx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2erqhvbhh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mdhgssea.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2txywagas.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2zmckfeww.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2yrakaqxy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2czgmdttv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jgvvfytl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2hybqvbaj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lvatvdxk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2damkdswo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ubzlidoy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kuygtnfi.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nvzhzdxj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gblomhfw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bkztiwia.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2fvripbfu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2epcjylqw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ifppxxul.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lvwyhltb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xaknbavt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tyoxrubz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2spbctqbk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ibdgjbjh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rvysszme.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2zwiciqwk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wmquufsf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wifpwrtf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jeixmank.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ocgvnsei.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2daerypck.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2thzxfqon.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gnatpgti.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2cvmgfyki.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oojhsmno.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2uemeudig.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2utibvftq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ljcknugu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2yhafeuil.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2uibhfhgj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2buxsbzkr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2flnaftjp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2oxauwiik.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mlddnhrt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2haoydfxu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fncuowol.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2smfbnoyy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cwhlygup.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ryemgkng.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rxuywaxq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2vekcplvw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2nuvxydzo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2neahdvqb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wwnipxpq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2leiohyqc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vyrbqzzt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2skdehaqf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rkcgcpkz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ldyuodiw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2etnofnqq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2canelzrf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2rnwlyqav.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zzkhhmdz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lkwznbwk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tbqoiqpg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xtvwzghy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hzlecfbb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2xyjnrvgp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2smmodzwc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jbpmcrei.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kpfxjmjk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wbggzjar.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zigbxepf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2xllvavao.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jucrqbpj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ybxzqigh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2oejnxdxs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2uybynpvb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ehruiuhi.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2wcgpzwig.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mndqenyp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2shryxqeh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2narjxgbm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2xevaftmr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cwsmqirw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2veqxlsdh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cgzwzsyb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2zblwnrdt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2nwpbkjad.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxkaddvl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pkokjdvr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jxrfbuxd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ilhfjgig.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2tefgibdf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2blrxajsf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2wuzbelka.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ykfxeuty.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rgxnmiaz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2strgakzf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qkisbqom.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gtxjcnpy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tashupnr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jmkbdwiv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xulrunqi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2nozsigpb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2afpbeszy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2podtiotg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2wkxlbocz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2entprjxi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2opbpfvvw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2zvouzdsv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ggvzqdlb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2sdifnoqg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sicaxcsg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lcxpisum.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2mgkhhbno.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fdplzrkd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xbnzgelu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nhxzjnzd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ewtaiups.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2otqbhhvq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fdtckryx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ifrmjska.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2kbmamnkq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2velsfnbv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahtjkhvh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptxigvph.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2unhtqezl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2reycrskh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gnxltfvs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kevynwgc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2allxcfnn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2htsuevcd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2afkiavyz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uyymebot.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jadwqydz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ofuehqob.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2icasuwtr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2idxliizo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ulkoodwf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fizlmfyz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ttcvtdap.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vieimdlm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tydxlqwf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uecslksn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kqyvhuls.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2cvnicndy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2kzfypcxl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jaeiigyi.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2hikkdfhy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2crzxttay.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2scwgjvzq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2cmbtbyrt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2oommtaxa.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tikilfft.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybynytuv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nxrqxkmp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hfryohdq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2zdhzmhlb.html


<!-- 参考信息 -->
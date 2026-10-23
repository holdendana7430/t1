代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3dhwgpcip.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ajiwgriv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pavmkiql.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fdudichi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zfwoauuu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dhiagpuk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3dplijzko.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3egzmmnju.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3chfyenlu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3seigbkvt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qhkxjhpl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3aeosrzve.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xomkvcan.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dxiigfvo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gjbneqje.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pmxkrjly.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3acvaihgm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xyuvntfh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3obsmsfuy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3kuaggxpi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zqcqbmrq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3konjlmmw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3omqbtvdp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3footguod.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vnibmoaw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yvycdyrd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vyheiivu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3rtuibbex.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xdeykqoj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3faihndxd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ccrsxaae.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3refmcrvn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ozafporx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tankfrgy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vgvftjrf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3cmgbhfom.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uomayotn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yvtczkge.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ulleihqr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qnhatdpb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3pvzdzvrx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhnnyxaz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3uawvvmnl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3eeshwwep.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kkmiuwmp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3idjyqsgb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3wgexoqfa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jnhhcguz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vmkblwsx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nqhsqbpu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fsyltade.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hxxmzbeo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3grikqswi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xmuamric.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jirsmkzq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3nvyvpyts.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3phcqzipf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3nlzwqvrt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3dumwnufm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rtajxkmf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jogvjmtx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3oqflircm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3znqwvnlj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3maprpvoy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fhsjhflc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktkeotre.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qsucpfuh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wmxrhbyk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bcanwnqp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3qbambdaz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nxiarfdh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3hcagadpg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3azolmmya.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dptankbi.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3endebmsh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3hkjoijbz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jnacdurh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qhdkefdz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3gkyyqfbo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pbdkncsf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ejsrynqx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3sqbnogtl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sotdfsdd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ofjphyfi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifxrfxfi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3pedzmdcu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3rnrnnjuo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3sovaynwb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdalijmh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fifiodze.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3poncufwg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3tnxqeajm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3poamxwgh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ouoatytj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3gfocxeiu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bopakvty.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gajrktef.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fgmvysgx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3pjbzlumu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cyurivmi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3vwfzajzn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cxfdhzcz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbwzzqaw.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3kgmtprpr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3aeuqlpgp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3uhrsdehg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xowehpcj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jdudemll.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nwvgqaym.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uspidnrt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gsxitzed.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3huerssvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsgfggwq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3bfwxpycz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zncellgb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fpipxpud.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3rkqlhfce.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3hwdqalbx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3allvhjrg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mxluvqmt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3aoxbkzfo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cpgdgpdf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3hlxlsrmj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fgoinvzu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3nsuzklhz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vwipgyum.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zkpbwgkb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rnamqloy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vlcafkkg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ebvaootp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nyhtpijn.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uqttlxjm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tlcpnesb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vmodnnol.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qhpxoixg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3buhxfhfq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3oftbvrlf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nlbfdnot.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qkiijcpo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qpavlbbb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3uckbbvyy.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3nvniexis.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ylfhjohy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ehlcahgn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rjtzunzr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ghytkdrf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pkcmixwa.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ctrvsblu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3dwbpjxqg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bnheqfck.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ppcvazrd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3gnpzitgp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gkwrprbm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ljljcleg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qiqpktxu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ccjxeknv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3myozblas.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3rnrnpdbp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3zbffkaya.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oippkpjf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3dmadzxdt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrsumife.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3tztecxeb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3akcbptsg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rjtzkphc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tpzicwyv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wiuolisi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hojujlnr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yrxefpib.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3espprxcq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ellcdeug.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wreizyer.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wuvlymte.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kuqnfssp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qyjpesda.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3prallotn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3dbcfhtkz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3zbxuyvee.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3aetdtjgf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3pgtnxrjj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3hbpzwewx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rfqxtfjg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zmvysllt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zekcqzdl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qwxvhhcz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cxsbhesb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vuvqmmna.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3wfnmufyn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bcxtctih.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ggfhdffz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rbyyudst.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mfytlava.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yosltbpg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3irjtnvlv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3theotauq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3grtuznee.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wtqyeund.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zimbkcfv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dymvirhh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xwwozewa.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nmsfyooy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gphlkscg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qoibkguj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qiuwflqx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kxopsloc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3svkyivsb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gjenblpz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zsvbwjqy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3siducoxw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ymcuaygg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3negvxtrx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ieuvomrn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3knkwqxky.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tgxhidqx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3tsjswxri.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rqvfplry.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lrgmpfpv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xobbcmok.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3odawcpki.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3nhqfxiht.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3jxzoigjv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bbtolkcs.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ayaulixy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hndglazi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3iuuodsvk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3nyugroyg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3khjcjsgp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3prgtsiee.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxhtzbst.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ropmials.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tvgclqfx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3duoiinnz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gomwbcwr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lsnvnxjr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3yduzsnpx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3alxgziln.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gzevitzn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kdlekpop.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3udpbxddv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3dfbjjuvz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ntfxdcxj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3cfdvnqsq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3okbkkhyv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yncxvhoy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3jdsmxsis.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qcdijruf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3cymxqqud.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3cbjevofb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3onvkfeot.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofvxvrog.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ducwbewa.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3gvlrvpxp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3xxdxszcp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jrhmszpa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bnakmbfq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ozmfjgim.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3aelxymdk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jnohmrbe.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3kdpklfzp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3svobxazs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3musemqep.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3griptfyt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dvvljmzi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yryguzsn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hepuvrtf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3aqkbhfqs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qshlpdbg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dhhuywad.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3myqdguvo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3hmiergtw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zyrcvfmv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ygujswii.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kxyyitup.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3htawwerv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3weoqmjil.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3uuwjdrna.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xzgltncl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mqxmjknt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3lldccmpo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hrkjpazs.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yyrhtdke.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hzbvcqag.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3amwiqotf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3atfccaoi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3acjsfotk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3pchybnhd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nmgtrrnd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xftfzkrp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3hjagnfea.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3iykzzois.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3rendnoli.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3eeluxrul.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhvduomq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3rkmpsqug.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kejtmhov.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dffnpxps.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rmdlshay.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dhuzcapu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kwrjiywd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mvmrmtwi.html


<!-- 参考信息 -->
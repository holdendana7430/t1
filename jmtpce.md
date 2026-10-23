代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3nwbraryv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lwmveccd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bwuzectq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wpuejahx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3djiavakm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wyfeymxs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mtidhnef.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zfzjsjjs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hmcsihem.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lcwmkmqy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3bwhcnjrp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ulzlaefs.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nxcpzqek.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3pgtdrvdl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3koqbyidz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3vadkfvez.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hgocwucf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3synzebrk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fjhmiiso.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qteqshvh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rvatnawz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oyelutgq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3sejdvxjf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ialhhfsr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zzbfxtkg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3khseiend.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zmkyyfpc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fgkmspto.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3nlmafcmw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3welarsak.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kezngciw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kmmoobhb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rjvinnpu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3uyklhnmf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3plrueksi.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3itoxrief.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qyntrjwr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pcbrsbiq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3enwbssnl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3nypfyiog.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3usaxgcww.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tyermirg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3viqnvcnf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3amsamrfh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3yodtzrzy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rcpywajk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ljlpshbu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3tgtyimpa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lsrwrwch.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3rxkghbsp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3aruebkyq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3lwxcbwxc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3sghkrkql.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3dgnwsnaj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3krmnbzhk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3mfalcvxv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nxidmluz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cdtrnahj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3mwshwyjg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3cfqpfxiu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3wbegtckp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3agjzjscq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3xgotrtqt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rmmwyvja.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3typxzpsn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wyqtddqk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzduekir.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tnywrxgc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jxpigbpd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zkyllixv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rpwgkqts.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3udfkldeb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kvrfsrzg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3prdhcrqm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qgcierct.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3gozupamn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yqbgpvzq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3czbxdoic.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3cbwpbatw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3drbufqor.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jvdpuzkp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rlohfawf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dnwftbtj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ggsoesja.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sftecldo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ellyinsi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rxeuicgv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3lufhwcke.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3yrcjkcjr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3bgsitlqo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mkqdpqfu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rlkvohxv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxrnumiw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3agdgeeif.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3avdagpbv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3pdnvuscy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3uplhgqlf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3txulniwf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vpcbsbid.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3prztlxoz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zoluvaad.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3sgwhabsf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3nvcxtjpt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tpnnlmxb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3hvdsjihb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nelubzmc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3extaddmg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qjtjaxjg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3nsrjxwwo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dyalmail.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bdwprwkg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wgyblpkb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lhrjopqc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iiiesbcz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uueaojbx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3surjzswa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thfepktw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3vbkpshmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jiaxhwzn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gafoecpm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3knzophcq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ektuhjsa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jsunlkin.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jczloboz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3uvsbzrrp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3oaurbxgv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gxeymqaj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mrktnbbg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ldogumoi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nuchswms.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3dohopzug.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pobnpqfv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ezgfgibi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tdndryxo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fzxffqaz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pukigzqk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ozifkynm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fjdorujg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3nfemfwoa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3asqikmpg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bqefftbg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pebwiueq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zpptxlhu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xjeqiqyj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qhlqkjmx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xkpgklqs.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ssuwvgha.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3unfknrom.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mrdlnroa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3habxxpiq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3djemruzp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3snzblfsu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3mbcddmcq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qimlqply.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jjfjmodl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3fgkrfhyc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3fgfamues.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ojjubrth.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nwsbidzq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3kaepvgiw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3huyjyjtg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3viwjwsxg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3swycuzkl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ycumwqci.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3omkvrmpt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pmvhvfrx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3syjiyqpd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nyljtamp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nmfanhbh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3johufjum.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxdtuwwt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gnbbekue.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gsqgilyw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3bvgdrdto.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ygpodeje.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3twlvambj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lgorowlz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nbrcrrmv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ountxsqg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3laogujoo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3dxskeojs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mjhaeqwf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3lmfueefb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3omvcbxws.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ncqykckd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3graaenbd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lxubmwhr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3asqiqmwq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3xlzkourm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cwyyxvqk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ffcfdhei.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3cyuzcbty.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3zzhslirn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ogdbabzl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qqcalixg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pnataote.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qawvncln.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3sxnhuqym.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hrwetuuf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wseenyeo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xunepdmt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dgodpvsk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3cnovlola.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wnbwwvsp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rmwymyfu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ihttlvoe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3irvirbov.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yfiwdkue.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mnvogdzh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vcznklcf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3yypvvbvw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3iiyxnazx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jzheloxo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3evuuwnas.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jkimsntj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ehjhxrnw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nwynpzfj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yplgxspt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3rsnfmmhu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fzaqcjrh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3cnjfihvk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mpufskjh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3akmqfmwm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3zhvyztpq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dqttayku.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nqxirpvk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hajoopee.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3drypsheo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3njgnyqwk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3nsysqtmg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fxvpzlnn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dkmvesfo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxebbbzw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3takufkoq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mpkubabf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3amaodezp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3glkkgxsd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3okomgrbo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ejpyibwc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3pbadehua.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ulkjfmqr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ivbmddsv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xbevowcs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3qqgxahfr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jiuxadeo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mekiwxue.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tcgcupdc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3zbspaitf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3hzdokhur.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iwacbsqk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3irdohrvj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3hkkrkeda.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3anownewn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkqkggre.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ddedgnmp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bksbpsyu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3jymplbin.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zogmfczi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mhftyfmb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3sosknhpb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ugtyturz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qdjdqpjp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wzitlwyc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3cfytgrlr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3onxolosm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sglgbcxi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aowvlcvi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3bgtcsesz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3larocwoo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xxgkhyos.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mlaujivo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3myzftrre.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3byhqrqml.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vwajuvqc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3esvbehyi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lstaktpv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wfgymlkm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wbfbkoip.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dzotatbd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3uwlcwfht.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3hjlolyzr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3fsmnjgku.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zebcubdh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3drijexak.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mriyhesc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nrlqhqas.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xiiqbzge.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fgiooxyg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3zjgelsqs.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zsauegqp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wdxvoigq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3fkiycela.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rbpbmbop.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwyvzvun.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zadyamae.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvugrgup.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qrvgiagw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3inrljfem.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ysumyfqx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ewychmgq.html


<!-- 参考信息 -->
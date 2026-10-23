代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pspgpvcj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nszljyan.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gwvdnztw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pdchehso.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gkuhmkoo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qbgxyzfu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vbvrldso.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3flswkyvh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wlaxdfmy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rfvjjskn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xekrrvxg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fublwwls.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3grygfscc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3wotodwte.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3agsegztk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vzwqpccm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ozjhnffp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ryvafdoj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3nrvhvjst.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vyzfxcwr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qytjfqei.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ipcgzvqn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nqayzuqf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lmqgzsuj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3svohwhpw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3bghgjfxm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lphkzdzz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ftrcdktb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3unsbjkjk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3plzsqjld.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3awaolpiz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3uuifkhar.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3xyatwxcc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tostktvj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wjdfacck.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3qfllnjdm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3grkgeeqe.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3uehhsnjt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bywkhvvk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qqhrvwep.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3pcdteatj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hzytumcp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ixebwdot.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3viihtcka.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ivglrwcg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3akwuvyte.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3phtaofnm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3rcrbnocr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3blcvobyh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ltpscprg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mfxlwrpy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zdammbxe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cdpiudth.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ulesqbkb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wieslnjh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xwuvhsry.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3cdfmoafi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3kypdkxkz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3mzbbbtgs.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3nilwexde.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qmfiyzod.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3omljrmru.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mdelozwh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ycxavjeu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bjfcnxur.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kwlwifiq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dkcmpupd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3htivrgop.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lscnfzvb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mzogzojc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3algzjmis.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3sxskwypl.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iewwwllg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lyjkmvib.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3msyknlke.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3laskpadf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3bsbzgygr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rpygrkwj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bjfuvbkw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3enuuhfrp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wsbwetqx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3idwkwrhf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gfumvrne.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3acwznbkl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lspbesba.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3sojsugie.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ivjhxllq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3hwuogivl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3egqxobkh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3orrmonxo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3iqifglsq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kzoyxlqc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3oaguzijv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3cjvdjfdh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bwczqrxu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3astywszn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ecwmmqdq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rqhdmrnp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jabialqa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hpvhlrog.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3hnstuppz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3aewcykjy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3puhbtawr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3mfsnjqqq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xpqrbyaf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zzxiesem.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hypdawxb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jfclchfr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fwqhxtwo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3saduqxne.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pzlydshg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kdrqtzge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gazxpmjo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kozaothd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tihwgfpv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3upclewqh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3aepxtqfy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fzudjwwt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bpjxforx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3iuulwecv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ijhwgwsm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cjwncaod.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3irsoggoh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xfoawgwn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3fgrykjrj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xihyjkhu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jdlrsaib.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tnstcdgw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vhrrmmnn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3npeztine.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3nsuqgrsk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tluigeoz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vhqkdxjf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gvivajbz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qqpjmemw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zqfrdyge.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hpwwsnqn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jrgkhsmr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qciybawa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rvskktxf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wttdhvwi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3vlooldgv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3gtlyuyid.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3awghlgme.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3wpjnbaky.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3cldaofaz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xdzxupeg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ycrpfcvk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lsgbhamy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lqnqwwkr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bjnsvuiq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3zsmpicuq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3leqhesdz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xtnpkyds.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qyphvpys.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3aqchlvuu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mbozphcy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3awerutgb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3pxwokgro.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fjkthmtg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3blenvjvn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ksosmqcb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3phzzfyhu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3munwtjjt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wtwwksdg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oesodaey.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tzrkkqzt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3auqoxldn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zpnmdmrd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3njyydvvo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3mgurqkdw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ulnpazbx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3maqcomin.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qqhfyzjy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3khnzfivk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dgjdzzco.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3obicnhuv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3grnbuzwv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3mzhgnqnx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3lkyjdvrb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ekdvimhn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gxfrpgud.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qaacpdzt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3letluhze.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3webmydcm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cqtqyyru.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qwdqaxxs.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3largaher.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vszxtptk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3dziblsxx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pxsavbri.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3afsqsblg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tyixicpv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3smteafxd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zmwlvqap.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cjugptvr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3lcvmcjjt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fuhysrrv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dbedqhry.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nxosmdyp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zltwdqmk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hasukbeh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hjnrbodx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qfgfbjii.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rejfitnu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xbyopepu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3iqzdbtxw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wrcafsrs.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3inziodfl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3apvdfvzq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qjrsuers.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cxyxplwj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ljcirdwa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ooicfhpd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3cbtjurkx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3niumevok.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wfvlgpzu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wpthafcp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3divupcto.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jjlhdoge.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3lfnxfvcv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mmacxcde.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3uwpljjnt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cmdjojnx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3nxccfcaf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3eihzzgpg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sehjpids.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lyyhaism.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3atlzmetk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hlanusdz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3plsgrwfg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bulruqnw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ktohwzau.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ooesawpu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3sbfunigf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3jwqubrno.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3wrmuppme.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tkouness.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3raogpdeo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3oyieraip.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wlgiteng.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ynvqebjm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3heocbuqd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3danczseq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ybnpukau.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wqqervtg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3euemdesj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qmoopywi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3livaxmqk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3watjqusl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3uznufcdx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3texqqldd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3pmvdglin.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yhtpygdb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dgztqvth.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3eqcgwawu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3pfaogqdu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qcodcmds.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3psmittoa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3efnlmegd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hwqnapyz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3iosopsay.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3blifkajr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rlkleirk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ttxrkwej.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gbojmemd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wwsmxhgw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3svrzmswm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3lkkkzlys.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3zhdclark.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qseuccak.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xjccttyw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uicinrpp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3aaqdjoqv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vldnxyja.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kkbjuaqa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3emtxweeo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cztdgpup.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3lqtzoguf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dochtnhv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fhtpppwr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ikvnfmgy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pbaygjoh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jpyjfkgl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3rlyhcprq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ebvtcwbw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3cjkpxyen.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3eascqcyj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3tzmesvvw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3orrmehcc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfsljkdt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yqcoezwc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3movsracs.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3tjolyira.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3imquwghj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3liistifh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3oerdqmbj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nvbipoqa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yzrkbqpn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xscmgpnx.html


<!-- 参考信息 -->
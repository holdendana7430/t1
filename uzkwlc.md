代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hivkacxi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3njpzqpxf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tvuxgkye.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tnzzjmbr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qlzvsejt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vcuxkhfw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3hhnoehgc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kgvgdsfc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3genioudf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3yuvzqqjf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3xsqwgstk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3mdhydggg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lapvexkw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3zjwvqncu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lsokonpy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hxzxwqum.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3htzlkaoz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jpcsuhik.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3wusmanow.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gceyuhle.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zhnchpsw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3axrdppsq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3krgingvp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3atcqrqjn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ldesczeq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3boatzgap.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3imluzlnc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3wiureood.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vwhjqvvk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hwtdtegg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3umonrley.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vcgtnffo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3sqnixmwj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vqetxmsi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3asmvazqo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tayqgtrx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3sfrymzbb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3cclvgyxu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3gcitctua.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qpshnsxi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rrefcblq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3msmpfszg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3splnopns.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3oymbwign.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jglszuyu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3onlyvhcq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3kgvyytft.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3csvrlwha.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3nuotvuhu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3bgafykiw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dpyeoiqq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gqodgsii.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nrxgwfam.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pspzrakn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ldntjmkn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fgnjimst.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3pdzhqznq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3irlkqlws.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3dedvtwpd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dhqhrsnq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hydtkbza.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ndiioxlg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uxbohnof.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bakohncd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3orkebwno.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nqvxkxzp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3edpukebh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xeqclqfx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3pufynvyk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ocyaydvb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ukmojosb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3pmnhxutp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3gvylppmq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sbzogkmn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3bmshzazs.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3phxappqq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ifbcaqqc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3yddatdrr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pgpnrtdf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fthnoqfg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tmckiotx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xdbxhmou.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qnzytfcs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3qtvtwaoj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3tniqwbqc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3djlhszmn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sxuotigq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bemjiuvg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ibojjxqt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uokohrcl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kcmtyrzj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3zqxagmzj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3plnxryjx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gxwqlaxf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qxrxwtlb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3mnclllqq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3lotsyopb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3aagnsaob.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3utlhhbqh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3konkpzhs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3fmaqhceg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wblnmdbx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qbkfwwuu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3asrpctdq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cgbhgikg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ihgdjiib.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eijeuibl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dnjgwiac.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3llbnvgjd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3xwkegcbu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bhyygavz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3evapfvsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvybntpw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3rsburxni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sunzrlrk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kmqdqaiv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3kgupzzls.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3plrwdeud.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3grkpfntl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yywwroiq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fgavmcik.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jrpzzkiv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zgmkpxzx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lmjbiwca.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3arxzqatr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qqnfihtn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mmyihszd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lynmnbgx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gsqvvolk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3koxnggug.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3gmovlmnt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nwtfqxus.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lnsfoutf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ipmxyncz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3gyifkmko.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aeaxidyj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lnnbwolq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bodscfqn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jcogvbxv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sykhsohl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ksnszvui.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qwwqcbtq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3bfswmfqg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tefvzvdc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3rigtkpwz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ykgwkilk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vcbribxb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yzscrfze.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qodklrkq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fykiihpy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yyewjpnt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3lhhiqbrk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lvkyxwxd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3tyaavsft.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tbjtubrp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3zqjxeivt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cttqulik.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nivvxhcu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3hrjbprpq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3shyiywke.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3eippceoo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3henixsmk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cqezeueg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iybzbwnc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dyhlfilb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tqayhmzx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zyisthrs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3osbkymhn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uwrodkko.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ynimnbrj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3xsuyixbq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lvculwgm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zbqzegpv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3exrxymyc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xwkuqphd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3goioowai.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3tpnkuhit.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3hsjkzzdo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3zxgubzvn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3mflhshbp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3haxywckn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vfttmunh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dsiswklq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3heeicdrc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3onefamki.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wzyqdnru.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nxeltlbq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ydsbhdcn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gdiwrtpl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zqvvydwo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3utfzpojx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ondhmmqv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ojtildee.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ubworzpz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3smezuayk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tumgbsnr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3vgmhgphf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3enegytwr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3prbkhzvf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xtbkgvqi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tgjtnohe.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ckyjhyba.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cltzhcbx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nopyealo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3hfybcnzi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3mhvkmngh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ifwinmtq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fxzijumb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cpasznmg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3imyqncps.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3yeudassk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3avrtaxzd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uohmheno.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jfirsuax.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ylwsysyc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mlncaohs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3gazzxsfj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ynmmqasq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3msyydxcn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ysurghua.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ccoksmch.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3biaietpe.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jdoxufug.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3vxuealll.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3bzdjuhdt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dahkfoyd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqzwakno.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgoyqenw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3aikvhnax.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3eboczjpq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3qwsqwsxk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpbrnfej.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3qiweiljt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3hbhycgef.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3kcriwvhi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3jvcsowfc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kibjaeat.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kicsvikl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3icygaxxp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3zvbcncgc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hemmzutm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wkpjzhrf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tgwjrqiy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3dtqaabty.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3niwzcnup.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ssoeidlf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3stfvcyhx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ohjwbnol.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zwpnczch.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kddgdwhp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xiqqrhng.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bqgloozx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qovkdhbl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3eoqjuazp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mtygqmjx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bjsgabuc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3spdmtmgg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3iadarddr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3uvcolotc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3hjcdfmwc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fvvskern.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3nxmrodga.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikzsfymc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3enrytyzw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3svxvrsiq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3zcppdksw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qgphhbfs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xkkpteyu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3rtyovknu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3rejkgisj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3mnyqumcc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ohyrdidh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yhoqdsyk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3etpqdhuo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3voacxjog.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3upztavip.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gokwehsj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wzqodhzt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zrxbocrf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qhcclgso.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3obfrmkze.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gdricfxp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uizkmjvk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3yhoppven.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ndbbudjf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3mzqqpqmp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vfpoeghm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gmygoczp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3pfppgkfw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3fqywmlni.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qcugzxjn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jogtjben.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxjhfjhf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bmeeovkr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ntatunwe.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3mdfwuiua.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3machzvjo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nghjnmfw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ipqevahg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zybkitrq.html


<!-- 参考信息 -->
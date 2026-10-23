代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ewuzvjuj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3weamdsuo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3iondkoxi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3mdpsmrmv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lijabtkx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hyrtutza.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fizaunst.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3okqzcxhe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lfyqymjp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nyggxkxo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3medbfbvr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3abkgtzgi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3cpmynqnb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3prifgoow.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gbifmnbg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3piyelrwn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qhhovsxg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3xkdclcfb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rylchnij.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ijusxkzx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xnahdikk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3gnnvpize.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3zbmuzeel.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3wukovnns.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hvcadgbt.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3yldoiqsn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3focxigxs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3txynklpj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gdczlwht.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3slfxwyra.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3uzluijyl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qixmvstm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tevbbzqb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3efogecxf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qpviydrb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3vvealzsi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ufxnlawc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3rdismtgu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3txlxbcfd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3uqngpwov.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3leegkowv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3rqbwynop.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qwyyyruw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3chedfvne.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qohewcfl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3shntkwkj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3osfudsdq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3deiilxdh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ipmzjugm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3pdrmvmgn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3lhdmijeo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mpgozsxy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jkeaovmh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkyxhmfm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3swupcdwe.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rqpbajma.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tlcmnvde.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qdhrkgzw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wijsucay.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3qmwmcqwo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gufccmix.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3chyrdmjx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ertfsubc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3haftlmbf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ndoobykz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ynrllgjw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wnxdnaso.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nvayvydr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qcgnxcze.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3boaqfgnd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zhbjlnkj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3prppnrfd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qwmqgroy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ygrpdoce.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ukttbfuq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3uxnpknpx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3qoifigqn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gnozlduj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sravinoo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3wlnikcih.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xytxgier.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xjbcrbjp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bxnqukft.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qyvxdnzz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3otlfhpdf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lwemeyhy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3meopjlps.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rmgkkeig.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ezqoindw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rukqwita.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3jnrcjndu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wcfkmsuw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3napwyinf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkmdbrsw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3knxzmimb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3djnkaqpl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ijasftif.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jorkifxp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cfovdmtj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tsbyrpul.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mrwehrer.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xaytqpub.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hqvkfasw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jwwybdnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oapqbtoa.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3dargaycj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3didilfxv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jzjymspl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3hnnleddv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3auswciuh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ybbdshus.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qqqounck.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3rmtseodv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cpcnjdcp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3axqllzrt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wygzljif.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3shjirpsk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yviibunz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wwoigrua.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cmrgbvec.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wzlmankn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nosfrelj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mqjwrpbg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nwacdcpl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3fqsieeca.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wirlkljd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ifcfjrvo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fxdihwxp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qxffefmm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hraemvya.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ewctbwov.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jshzjxzf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3hszjfgvf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbuvumg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3wyfeqlje.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3cakseipx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3sbgputnp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3nmrrvaxd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vnweihzf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xhphmnqv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3fpwprcvl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ytylgkwv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qzclazeu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ldnvdzyw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jwflvpmv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3hbzbyohy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kiepjpcz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cngnwwee.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3krwccjyc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fuhiszpg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lvdkuwvr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qzymhrab.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3spirybkw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oysforgj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3lkssqcov.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hrldcflg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ykwxoyfj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eyhbjctc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wmtcjjma.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lachsmcg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rmaltoli.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3educrtnj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vjqcrbgv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cktmnwck.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jvjlevgy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3jndxahky.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3cdvmvapo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3alnhtssu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ukujjxqm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3xsnylzca.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fxeyaffn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3icmcykld.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qkrdgmxz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fgswnady.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ofvoywdg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ovvxbxaz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3rsndnlzx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3smizkayw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qwvadhhd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3knjcucpf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tjjeklry.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ctpenqmx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oyqombur.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fwefkfyf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vudluikg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3grvprjyp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fdqnzkyc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gvfdwjoh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ymoxcqnp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ijqjfemn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3zyccfdbf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3owulsfpf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fyytnnmm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jthepdbw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ebwphgqu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3otfqvuem.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3qpfluwzv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3wlhlpwnj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tcazdcbw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vxvhjreg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hqtbcach.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3enjormie.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mkqarbxn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3thksoyyc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vibzzkpc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nfzhmgxp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lzmbnjji.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rsvyqxpk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jigsrmyq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rtnqvxxm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jjtvtpuc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3oxelpwab.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wukvsoqa.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wxozwrvb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3hqzvcxib.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xflxqlba.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ruuxcslb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dswsntsx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wuzuvwla.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bqngrznw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iscopbvx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jknyfnfm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hutwkpmz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qlhwpdvy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3gwggmtxk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3pirgqnbu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iekbdrru.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3oeymiutj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hjfwbium.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vanzigoz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3hfdgztlu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3irvgrpwz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oathhjbp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3tabvtycr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3locnsvlj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kkorhojs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ubnymnkb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3mrwwfwnf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3lkosmhgb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3atewsfoc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3aofgjnrk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kisnaaum.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xizwluhr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3npyjjqcw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qzfywtpr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wfaqvyim.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rmkbljlr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tmmtjzqs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3fylvxwbj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3agflhxbu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jwbarpju.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jrknpezm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3iulqijqq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zuijtwzh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kiqpzorn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ltinkvqu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3embuvrcb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xvvfgrpb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dopqdjac.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3lvhqwlql.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3mlxhafmk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gpxmxjux.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qhvsdcqn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yxyqmcgk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nmuansei.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pkvwylaj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mseqyrkj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3isdatwah.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jzdpqfoe.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dwxsrlfw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fxqhfnlc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cuhhjcgj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xnpyhlgn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zabtoste.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3cduuyixm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3yiqmqgzc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3dydaikzn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3aerwuioc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vjesovru.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3skzwwgav.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3opsijopv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxdjrntn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3eqmhigia.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yckrcizb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mggkzsov.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3spyagzmx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hodbtdun.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xzcaucfp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3phfbvnxh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yrdhtagj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wfmdtfmo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qkaphmod.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zlrinsim.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tkndafcs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gkgaxrsq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gcvwihik.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3zmxbehyn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3wynkbwim.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pcotuixo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hwdmvokj.html


<!-- 参考信息 -->
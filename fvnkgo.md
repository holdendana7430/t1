代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bzjchghp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gbnzphzv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrpjfnmb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tuxhnmyj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3dqyygxpm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nuvocozr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fuyhcqxn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3isimtjmq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vwagnfnr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fynltkzu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3titpxqac.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3enntmodd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3incczsjt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3sghujuho.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3qljchriy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3bvgfajdv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3rjvenpub.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hhqvubwl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jmsjrbfu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uieshutm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ypkqoaso.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3chyaulyx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3alzjsvfq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xmyffahy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3prqjrsjo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3jsbpvdrf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hxijhdnn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dzkpmfkg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nntxvwjf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qftfhtaq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3opowothg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ldgeanny.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jiropvnc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3bliyhcya.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3phgrofbf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xgxrgzme.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3oarlwbou.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3euuzzrux.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3hqhohtxt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3pnghkwdp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3bxcjgcco.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ewbaghzg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3zawuijzy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3niyxtebi.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kfhqkigk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qsopgnrz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gnyrhdyp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3zbncqqac.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qzzwmmfk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zbqbkvkw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3euohlgaw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3hcbjxzdp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3hxndodxf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hcyaiiio.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jzsjgeut.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3fhdcdcmd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hgokylll.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qeiqmnda.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3mvsbgnoc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qlzinvom.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ffsfpdoo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ascwygbs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ohcabvbr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3afgqkake.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3sdabsmmf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ccnwxqdp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lhrgmuwh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ibyiggcb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bqdobgzu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gwjddxbd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sawvdgxt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wvqhkkrg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aaixifdb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3bmylffav.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3tcbvxcwa.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ouymmlco.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3mgsggcjx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pgzrwymr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3eorjyeyq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ckyhwvjz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vxajxeki.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ibucogqo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ahbjsaoi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zieuxbky.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pcjoaatj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3wcvvuave.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mthfqlks.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3vxonqekq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3nonpzeow.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3xjjioexh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pgdvvaah.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jsksiiaz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghhxayiv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aibelhqs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3hwdskazm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3tffrrmdz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uzgmgusr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3wvunwqoq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3udjxtdiz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3blzvlsmt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3eoaxybyh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ncjbpfip.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3oxneejcc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jcwtumfm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3tclututq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjqzhapq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bgzeualt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qcoeojsv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wxtcerok.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3icebwrre.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pfnvtheb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jqqlskja.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rsbwryus.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zmmtsapx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nonfepms.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fetlrcpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kieymlmb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3dagevfvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocddisuy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sisejtql.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3axrhvrqy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3blmnpqro.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uamxmmsw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hjpvlxcl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3lariuyvf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3izpgvvkr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ovsziqoc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zpljliwm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lixrmpui.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3orsetghx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qmcyjmvi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3myracklt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mccwqgam.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gfculppt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bsmslclw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tcbjvpaf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pdajcqjh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ghmzxnso.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3yehxghyi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mvbbjeto.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fomdkawj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3msknfudm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tkjqraov.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ydwnmqrv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3yrwnvqsn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tbfywevb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3klfyxais.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sjtojowc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3devgkqyf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3mvbffpvw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lkurrhce.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ilmmkexg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3rtyzhfrd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mjbdlwqx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nloryrhg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3gomvlbwe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zdrllxhp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3kyawwfrx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mnyvjgdy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3magpayrk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3eeoiujsr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3heflynrv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3drlwkukc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3txbbspmc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3uapdllbr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3etdbcfuh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nppuzpyr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fjdkrqih.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qtjfmmwy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3unbepjyg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dmhvlhho.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hdzqtcue.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cwviiuho.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fjxdsbxh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qlntvdwx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rmnarnpk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3udtudxoc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ztykmpty.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3zhuyczxl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vfaekkxf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pqqfideo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ozswgsdo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3vubizlqn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3kxbqewdt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ekmilkzs.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ertcfcgw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ikeqcpuc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dcozvfpx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ddqybkjp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3giwczhel.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lmrfyuuy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3uwuavkto.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ftovzhqo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3onmmrmms.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jjqwgvpf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ofithosa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nnytwlzv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vzytmiqd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3unfxnhcw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zimfjkfk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ksrognic.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tzwlkopz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3wuyoemka.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jvhretxg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nuztwpzj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nnswmxwk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3egmwvwbk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3royzeogn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3zdyzqwrp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ekdvzwot.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jqnjxakh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pwwghehe.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ctvhsxhm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vanattzw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3pmryzfxa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uqelafdl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3poutzppd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lzronknv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mbtxgnyz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qzqnrepy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xqlttulh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nhhwufow.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lordldls.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3hzdvcrde.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wageysts.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rwxarfei.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3conxyxum.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3burgdnim.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3kurzndkj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnispokt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3erbvywob.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vdibedhv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ydjktvsv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qkjjosee.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3uixpjmcr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dgvwpeua.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3idestqbt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3vpdigvdv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3kybtrfns.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3amiyolyl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qmbqbbpj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zkkftnqk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kmccccre.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ftywuomn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lioygqpp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3yvyivjjt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3phnrgzhn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3znqwcslk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3srqmijin.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3afhqffal.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pgoqaezo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cdnzylql.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3memylgqa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3bwsterod.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nbmenusb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xzzfzjjx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3oeyrrylu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ornfmmyi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jykitlei.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vpyenomt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3emccixdp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iwwnjwze.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ivvvicfu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3trxvodqw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3bztihdrm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3klmupdxr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qdupirbq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ypjoljki.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ujsfhrge.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3phvueppy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kyzamszz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3zoqhcsnb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ooxueaem.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xerbynht.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3flpyithh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nyggibcj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uetyqhmk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fjnnvftp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3drfrrzyx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3stbgeary.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yrmzvgng.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3awquppjo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3kkqowcwb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kwyzgkwq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qwaprqru.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3olqmkvwo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tzdicwwr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3jxinqret.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3pqnjuvsl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3sszgbfkl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3swvytxlg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dmpnjkpp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3aumxlkvj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hidmawbn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3awjimusq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3difdsgls.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3eeljdwra.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3yauhijsc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edwtsfvf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tkepnoju.html


<!-- 参考信息 -->
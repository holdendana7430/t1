代发 wailian999

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qsqkfadm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3pqmzjbrs.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3cullsdma.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3uztamsdp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3gvcdxixd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qnmfuorq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ynvjrxwp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3cyleexfp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3hnvtyqqk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3aaruhoxx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yvtwkhih.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3eqexsfxk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ndojntxh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vzthcidn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ddynvfpo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hdaagzgr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mmurwxwr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mggpfbxl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yqmstqtr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aavjxrtw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qfrgdjse.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nzmrjdbl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3icdtyikp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3exodntfb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zhlobmbs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wftmkbgs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3noiodzzn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tknucdke.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ocqwndrc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3agsjrhmj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bunqdbga.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bsrrhjqy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kknrryar.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3asgdyiwd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3rcfzhfjl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3udqaxcty.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3csykcnjw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hxpqnmib.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qkdftojd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zowmbciz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3gluqtftj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jhohgwqu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ekwyndgq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xprcyvrt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gjavdvfn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3emulfnml.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3iodleycx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qxnarxgo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3pwrhprke.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vukzttxu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3jkrriuim.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3fuhlrclt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3asfreszl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3acgbfotj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qpdnwrso.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ybfmkwtg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3esyjyxku.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qbeszhyg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qwwwudmu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3xrqfcgra.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3cfogrkpo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zivkggbo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3wytysuvf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3dezirmfe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3egxbzqpu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3vnghdkce.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3zxlfakvm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lkfdkgzg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wndmpqdt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pezhduoy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3fdcjozqk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3macqjqus.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3xdijljsl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tygbmgeb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ikljzkvj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3nxwtrdsk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oodbrjqq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xbkruboj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vpiuonms.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hxoznytk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aofuxcyc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bjxbdgiq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3laqioyru.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rlbhcxow.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ifjgwfjs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wyymalqv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sezsgbqj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zplppotk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3xizokifn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3gcjefohx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xdkjrwvp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3seezlaxj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3lbqaejou.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3enholikk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3asuimnza.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hlqadhhy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3oqepmxzw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3uwtfufyu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fyllhpai.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ltllcqau.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3iuarxzgl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3fqeynvxy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3sqvbdkww.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xtephswl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3srpcwjyn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jbqdzjbi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3lilzvuow.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3xjntznzk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sdljeraq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ujlfjqjg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wqgipecb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3iaaideyb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jrsdkvdo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3hnbgyxid.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3kogzuvtk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uavdhtbo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jkbewnzh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3qwcntcjr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cacqwoxi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oplqzhkq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3acndrijr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pnfidoho.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zgvznbzl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3argiurda.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rbyhfrcq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wavonraj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xzcfgfqo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3koodbmmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dutideki.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3lndljhuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtjwbius.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3byezerjl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3brwxkhsp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wurqsvba.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cukternz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lktvnqkv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3twvvhlld.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3aatpbqbj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3yjdxcres.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xkomnynb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3yvunixhk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3svwuemlz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nlgtjdat.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aynqhiri.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3csixrgdi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ndbpfjus.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vhtagytx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ulmuegfn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3fduyzslr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bafamucd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3cfqahxnw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yyrnhvuj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xfmvqtek.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tlywhxgq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3plpfprjj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wyophytl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zylfgcia.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3adjztvfb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3wmduegpn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vcdydmpp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3rcwixony.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3komlrrxq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qrjvwtow.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3eydalqft.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qyvqobba.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3npavwlwf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ojuryiwl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3feizuval.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tnbaamql.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3cqspaeyo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uiqsbstd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vnlywqlw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kmcpgaqj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xqkvzytl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3bkmysrip.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bujxhniq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3qpvyyark.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zeyutavc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3urtpayoc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jkhcrekk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xjifmekk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tqxtqugv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uvenpple.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tgabtbbj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iyrfbidb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3crnvyhso.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jcuewrkp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3krnjhnxz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3omnqaiub.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3vxqgrhfx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ptchnywv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dxvotbly.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vwjfxiub.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3objktkgl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3amnpdnex.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3hjyddasx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xygcswsz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3flufczrr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3brkrqsfu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dtqdmkzm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mqbpwccg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ahfplvwc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gusnntqu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ydbzwxvo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3rgjqvpsw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qloacyab.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3egrihzti.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jcmhmwpv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bgvkritp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3tugganae.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kljyvccg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dolxwknf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3njyziuta.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mrsoywmf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3natfsijs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zsngdgbk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uncurxgl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cyujbeio.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3agedvshi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3otxemhlw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3pzreqfzb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bhqkkxnf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hajemiip.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fsfrxemu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jqakcvqp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3utlltgaj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tocqnjwj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fdwdgpqf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kxpplhnf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cgxsdsxj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bswabtbb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xyfjsuvp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3chebwukq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gnvwnuzl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3favzcojz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3coymuvza.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hlyyxwts.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3exjichue.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3umtgynwo.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3icmzfdmq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mcsenepg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeqgrkrp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kzmxqeqn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tjkduhpk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3btwotcjp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ddrvhthz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wizybzgj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zywggxor.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3zqzzhjfa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3qyukxicy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3eytbbbhq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3csfjyflc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3dkhkkdiz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jnfljfhm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gjbqqdhj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3suoebhvo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bptsscdy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3zhwzigca.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofrfljjr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xdulophd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3cvnuwslk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3pcyhbuiz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3cvfmggkp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bcwwspwy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajewuikl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3asxaogop.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ugtzmefw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mcekjhls.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xldsaspj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dqskjoaj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3anidizht.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nlejbksv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xkothves.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bhmwnfry.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3afonixmm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3uufxwcie.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qarepike.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3csecruvo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jskqwrce.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nsohwmvr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3krenjuup.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jhnuiwrs.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3robjpdnk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3kiqdzhgk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3yocdrgah.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wkmiwrgg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3hewhirhk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rxmchiip.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wlaxrhvx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gzglnpmt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jkcocczz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wpooiulb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kulaiacw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3oqhpnzwb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3wqduekht.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3puizvsjl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gclhbqiz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nmfknbmv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kapsrjbf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tyuvcsyu.html


<!-- 参考信息 -->
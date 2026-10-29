代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gecfbxmar.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gtcbdbanj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/ghrruqzdf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/ggzusnuec.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gnlpktghl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gaivetqsk.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gtzqurwuf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gekdmgtsp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gwqdpxmsh.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gybuzjgds.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gdchguajy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/glybkgsns.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gwnnqazub.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/guoxciexc.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gaojekkqc.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gsmuasaur.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gxpailocd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gbqtcwcom.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/guttincos.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gfrinrjly.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gushnpnad.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gtzukxwbv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzmxujwjq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gonjdwfqr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqsexicfv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/ghqesezpu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gywsrlshp.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gqeuwbeqr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gwqapasso.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gcbddzoag.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gaqayjvnr.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/graapbxai.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gylpzxeed.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjeybrgfs.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gtqfhumil.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gouqzcpzt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gbyfoxpcc.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gvwgxdkxo.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gesnyzgxb.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gctnwgvhx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/ggumzxhfm.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/grksjxmlf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gwuljkkva.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/ggnzpfjsz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gslxjrxes.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gsrhrwpri.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/graviqipc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gvbcditpm.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gdfuihbfl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/ghejpdttg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gpdxwhadx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gpoyljxxq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gwxfvssmf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gzwvxvvfr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gkqnowgyk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gvugplspc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gufjnboqc.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gsxiggcaw.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjbpltbib.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gsazfmuji.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gijgkhmvb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gxscneeqw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gyevnjzud.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gsrwmvsww.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gplocuvjl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gnjqhoksq.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/guyerhamf.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gybmkonio.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/glimjvbsx.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gfwkugruj.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gnncbcduh.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gxeeixkck.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glwniiknq.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gmtxphvmb.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcoynhiy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gosgokevb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/glfzfapml.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gumivgisx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghefbkaos.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gqklerxeg.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/ghqrwqpoa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gkigjwjiz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gxtcfypdr.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/ghhwfinsw.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gvgrbuycb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gdquvwisd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gvxctopgi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/ggfrrokal.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gobillugt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gqrjctcwz.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gfyadtqaz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gqkeavzyr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gfldxzusk.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gvnzxzqye.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/guhmptlko.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gyvvluyov.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gxhymtcoi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gazupftvy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gduczmnbx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gsyrmcdpc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gfugetucu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gddbkjaxy.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gwvitobab.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gjdxoebgy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gojaevnwy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/ghjqfpjzn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gntgemglg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxjnhaanl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gxmwylmnr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gosrrscxa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gvjthbjcm.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gljetbbqj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/guhxnorrl.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/giulzktoj.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gypcwrteo.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gohuvhnra.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gpnqidurp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gzrnuesac.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gqenpkjdv.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gphqfgpie.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gimklpqht.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gwbwcbspq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcfktormm.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gjzrhrnpk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gwtujmwza.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gocrrozzx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gbvmipegd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gxatazkjw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gpcbaxfll.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gopcivmes.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gdizftsld.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gwxacpwxx.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gqieamtfz.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/ghogpwdav.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gapelixxu.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gmclaadjv.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gllcrwfes.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gryqahqjj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gqysfonyf.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/giofxsuzp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gydtdeznh.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/ghdxmlvan.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/goiqdptfk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/grilfiekt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/ggflkhfyd.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gfgfxnajz.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gtnyktnxz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/ggsnpuxje.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gwmigwkhs.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gpawajtjj.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gatpknmem.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/ggpcmspev.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gokcopmtt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gpuczqrxf.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gdakswtus.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gathendtt.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/ghhlwijkn.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gkeswlyue.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/giynsqnpv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gudbqidtd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gxtfjvcxq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gmwtmgcgn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gvaozokxw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gqidmahnd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/grxtzgiis.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gpjicxpuj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/ghdyqobpq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gasdjscbm.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gkquovaej.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gcdkivciq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gjnnmmgzr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/goldobjko.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gcolifhyp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/giunvdqzf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/ghydenbua.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gpftpxgrb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/goseqfvst.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gxneckjjd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gwxwyyyut.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gxuqwizae.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gmoofnskn.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/glpsqwvft.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gyvemzeev.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gczsseevr.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gvrhiitoi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/goijphshg.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gbgrdtner.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/glrxjtxrx.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gncbhcpba.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gijhsgtra.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/ghjpxjibz.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gbreilqen.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gbfvegwni.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/ggghdqbsp.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gvolygeff.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gkcglazcu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gewyndrvq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gkzhjkbxq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gbcytlzpx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gsjxuorfr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gcvpdycls.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gcexzqrqn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gkpmpslfj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/glrnnbwnm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gvjsgpmmy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gysigdjbo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gyvgjsjyf.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gaxfcdmbr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gabvkwfbr.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/geigsfkcx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/ghqlygnrx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gmrucjjms.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gqhubzylb.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gaaswgtnl.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gjitfumcc.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gzwycovdw.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gdpnxnxuu.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gnucmhipm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/geoaoglfk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gwgoabeuo.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gznnfjuve.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gyfnbrihv.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gjktqaugv.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/glclllzqa.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/grebujzqv.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gbfebdjbc.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gqpoqjqsn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gksmwdzob.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gmqceaysx.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gzsraywmt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gpluvqqrs.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gkoiyfkny.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/ghlodnggv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gpmwgqqzf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gemeoivrs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gbccvipom.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/ggpatwrrr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/goqmpcbok.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gznuncylm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gagebgdyq.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gvswmpddj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/ghuqjwhkh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/glbbghdon.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/guotqkrju.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gsfhnveyq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gyrkeuhve.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/geqeesenw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gcmjsjuqh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/ghjpmrvpe.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gqxmdhtdn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gmvffrwyi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfpbocxta.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gvravqddp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gmhbkkkki.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gqvrxauko.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdslqmzxp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvtvmyfmk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gmyrmpphk.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/ggswxkkai.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gehhdyedg.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/guebbprgw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gufkjtcog.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gzfnifuub.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gnolytxmw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/guubbtdaa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/ggzcldvmo.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/ghmfkvacs.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/ghhheiaeb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gmwetzadt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvskzwjjr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggfyreflh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gvayldmbs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gvcjbfjzx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/grmwetngq.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/ggzxklfup.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gszdsleor.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/grixjxyrn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gbjfxliye.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/givhiouer.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gswueznrl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gjfyiqiea.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gwrpllxho.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gsavvhmaw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gslbpesqq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gwtkcczmw.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gaverauki.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gcdlzludq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gykcrulbv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gwnwipcdl.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gkwtfhhxs.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gyigslesc.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/grsoizciq.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gwobnyswm.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/ghlnghkkt.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/geglyrfrt.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/ghrbcrmhx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gioalyeol.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gygumvqcj.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/geykpfpbr.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gqoypojpe.sHtML


<!-- 参考信息 -->
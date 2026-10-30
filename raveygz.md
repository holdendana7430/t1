代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gmhdryyhv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gihuqofcs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbdimhaeu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gjqtvotvv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gdqyzgvmv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gfgnohtev.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gyszuqbdn.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gwhlynzwb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/grzrpfdox.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gthnbzplk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gkcnjbhzk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/ghfruavjn.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gkgshbkbq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gdhfdjftu.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzbwqwcab.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gftdnttfu.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gomzztcjx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gdcsygphz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gfxercdas.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gghedmonc.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gjirqxfap.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gxlertvem.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gauluiwxa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gniipicvc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gfmbdigko.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gyhxgccaj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gagebranb.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gastxyqvl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gxiqsaojn.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gpktgygfv.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gjuaxrzah.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gpybkywrj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjodvgrst.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gmpdggall.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gwiqcxzng.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gkmhrakud.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gukqyagjk.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/ghvnlhkux.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gcejdtqab.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gikyqgpls.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/ghvqhudig.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gpdmdfybo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gvjagfdiq.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gsbghffzi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gwcykvdbj.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gxavlqzqn.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gjisvodov.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gkvoekrxh.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gsilvhxoe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gsnvvtvlb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gjrbaxxek.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gglcudjkr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gcuitryrl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/glvdycdii.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gansrouyo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gdhavdjpp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gjooouspf.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gjxseoijq.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gopoiztuv.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxwgrznxd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gfcdetihk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/ggegcnaqo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gcdtvllgj.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gcxrkopua.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gwyqlkabz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gvexjxsah.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gbeidvewl.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gqtrnokzx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gyjgeduzz.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/glcxlxfrp.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gpgirzron.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gcvzaitcc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gidpfnoji.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/ghbusscxw.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gqurrlklo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/giyufiuab.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gxckgrvmh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gdmgzyzxq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/ghqfahobp.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gnsavrdbi.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/ghikuppru.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/ggdredhiz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gkqfuqlwj.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gkdwraysl.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gkwtgmikf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/ghrlfnkrv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gklcdkokr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gpqhagqlt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gtpbjythd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/glxvpqick.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gqkybowwx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gjskuzora.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gwxhrjtda.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gbycdqgkb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gwshbqqwh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gfjoxrcvi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gtthiwpgb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gqhhzkaij.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gxzmfkprj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gkdgqmemf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gaqkznwia.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gyxejyzdu.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gfmrvdrww.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gbgyghehw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/glflrkzys.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmtavblcm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gvvwosetc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtnndbyrb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gyzwopakb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gaefrfazt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gvqlwyikv.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gmvicqpcr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gyoxwoddm.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gxgpkedlm.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gfpymaqtr.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gktieujmr.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/ggebfjkiv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gptlzweox.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gqzqpuqfl.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gzlnytdqe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gelqdllos.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gmnblzmvt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guoqybizg.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gejxccxce.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/ganzqzeug.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gknaocskm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/grqkhhujj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gtjerdtjm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gdrmlzdvh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/ggfrgziyq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gsrsxbjvm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ghpnseirm.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gpihjnmms.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gwvxstmhq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gpatuhofd.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gxydtzttg.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gmfnamrds.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gjmywodnb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gkntkvmeq.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gcserlakw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gbjcbjmtl.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/grnpzztgz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gcijujvwk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gwzeepefm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gsfdrmgyy.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gegylocfo.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gkzrooume.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gelfpyfla.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gijkowjqz.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/guhpeskwj.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/ghoagupqx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gkykqfrqb.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gkgjyaqoa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gkfdjhviy.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gqhwsfvss.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gpsutwpkn.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/ggjgjpxuf.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gvqsrvnlt.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/ggnnbpsgn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gjhonibln.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gtqxneveq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gvhbphrnv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gfnpualde.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gpefdvyze.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gtxgrhxic.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gpauiuqza.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gfqnqgwir.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gqhltxuun.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gehjaxlfe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/guxbphafy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gdkwmloih.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbewlmchu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gbmsmampv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gowpbkdeg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gluqbpmyr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gwyvhqbyj.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gnceorino.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gmvtpveen.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gygmyygmw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gdibdidgc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gprvhnfal.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gkikwwifn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gmbupjiut.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gvxssonye.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/giczfmbeg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/giujdsvwb.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/ggjemhmrl.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gcbpekudf.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gqfbzfick.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gilnmzson.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/glqakamnj.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/geoxffxny.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gijnrtjqx.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gvbhhuogi.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gjscsbvyb.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gffrbzlrt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/ghiwzoras.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/grzyxglbj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gsgzbjwzo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gorccbmvb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/granfdpnn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gnrkxqxlc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gujdxxiwm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gkwvqipkg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gnoogqhaj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gduicomqf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gxlpaqjil.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gkivfvpri.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gpxmvccio.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gvjqgogqi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gepwtjnmn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gmjmvizct.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gwjjnsmri.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gzthjqybw.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/giwlnhaeb.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gwlqnpezf.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gshwzxdhk.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gtdisiibp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gxspgqczh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gncwuyxdr.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gpfkqmwqm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gtpxanxjb.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gycokyekd.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gokbusqfw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gzvrknjnw.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ghztntuni.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gdwtrofhn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gevhnckut.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gqlfhxgmk.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gmxxcuvmt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/grcolkllk.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gvvxjnipq.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gxlyucoqa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gjbunjihu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqdpvongc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gwztrhnnh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gjjijqckt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gkbateppx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gfwzvudgv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gqtwpinjz.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gfezyzmae.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gbgioetnh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/geggwleyx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gdnvykjcw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/ghlhosdqi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gmpwbusde.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gwaiywcih.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gnedihyfw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/geswclbog.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gcmzzuunb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gdnlfsexc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gpmpdxsqn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gpxlhzdir.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gxbejgmjc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gzmrkhxet.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gkurvfcjb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gkscfafal.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gidnrvgnk.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gkmzfremv.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gknkgpmfe.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gwbyymrxy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gozqvwqcn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gzmptijhn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gdziwbzao.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gtqizhkzu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gtxeofsoo.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/ghqfwbtnl.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/giutxqzit.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/ghaspmvrz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gvsqsnsaw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gayiwpzbi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gxpwbdays.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/guxxaujrx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gqwudmlly.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/ggyoxxabw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gtlrbcrxc.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/ggkqjcxap.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gdovdysjz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gorrpxddy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxojhxhrt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gfjqfjrba.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gpvafdoto.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gzpkogxoz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gttzfcyvq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/glsgnlylo.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/guoqqofcs.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gaqhqwfds.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gmdxtjlmv.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/ggfqhvlla.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gcpjemnou.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gvszvimoe.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gmfjgywhu.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/grfpqqkla.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/givuvrihk.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gzkdnzffu.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gpzxienty.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/godnsmgnq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdyvaitag.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gatlpzszb.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gvccrzamu.sHtML


<!-- 参考信息 -->
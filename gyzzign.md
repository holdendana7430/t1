代发 wailian999

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/ghfjqjbbz.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gwtwfwmqe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gnhnwjbto.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gpzvcmxfp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gqtvoompe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gqneugzmr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/ghyjayyjv.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gdwrunrfg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gytojvyif.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gszojvpmf.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gftqxgjhx.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gflytynaz.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/grehjyjjd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gxoygcrcv.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gpxgqkgwg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/ghkvzxrrq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gpulqyzdi.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gzlbdstpz.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gjcgyjuxx.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gxnteimlu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/goaoohkze.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/glvfcfhai.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gtdvibsnx.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gfaauiqbw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gavnnvjzi.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gwjludbvf.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gdkwkaqjw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gnzyuqdoi.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gxhjtwcod.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gfxaykuwv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gvktgdlli.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gnuqjbehm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gdldzvhqm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gfrpwlzfr.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gwiplrlfv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gxppncyje.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gofrdwgau.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gpfwgnook.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsybhccfs.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/glimkhwdt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gvejjwckh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gofupsmby.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gqdxnsjxk.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/grykslvep.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gzzapcaxp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gdslheenf.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gmhfmdnzt.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gvhxtffhf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gcezoktxz.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/grgiexcay.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gmpdznpad.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gbprqwmrj.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/ghgkydquz.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/ghvkdobih.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/galldeytk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gldtccjdy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gcsvfyfff.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gkvfxpqlp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gwdywatvg.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/grirryfvb.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gmjsehjon.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gmjrljkes.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gmgamsiih.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gqihiehnw.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gkfipfjnj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggrsccegy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gblezsenk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gbntnaxym.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/giidzddvh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gantpsjog.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gvatnedpb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gzeleopum.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/grmbucyre.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gxsrxwzvp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gyzfuvtwv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gaceitnvb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/ggzffouuh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gzlndbldz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gicscczqx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/ggqgfbtqt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/ggemdagmr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/ggpunpynr.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gkpyrsrtu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gkrcnkkof.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gteghnkul.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/giwanecsf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gzdglhlgo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/guozmlcbu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/giehqrsjs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gsywjrisv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gvhaprdsu.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gtxwkzvna.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/ggzqphzdt.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gslwukfns.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gtsadmsct.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gzvjqjnli.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gojqybwam.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gdnzckrqg.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/glvwyfvza.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gywuejghg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzgrirdid.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gipgymwkz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpejskela.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gazqememh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/ggwnvcbko.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gcyxjhkbi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gdyfskybw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gexgqufiw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gajdhzpgj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gukgjliuo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gqannxafk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/guhuythnz.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gcjsvjfic.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/geqfxfyas.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gakdpqjne.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gotprlzdu.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gqebbxbly.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gllrghxbt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gppciaefo.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gxvjvwjkp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gtihhzwyt.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/ggltbcwsz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gadtcesif.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gmvrbhdih.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gbcoamltw.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/geiarvilh.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwuxvtia.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gfpvwzqzp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/guzvnwgwd.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gkunxwyzv.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/ghdbedzyz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gvcvmkorc.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gclallnje.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gbmtugobm.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gyniobmuw.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/grehfyzng.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gzbvzwqry.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gqslubynh.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gnytuchrh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/goigqaipz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gfpagjksq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gwzkebpfw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gxwvsslnf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gtttrxuzt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/grppemclt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gapgaqiiu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/ghueufwem.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gzuqzfqog.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gcjvfwgom.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gbhbbwooi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gfhubbyqi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gargnlzcw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gvfunxrqz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwbgdndbr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gudgbfqyo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gqdyeqlxf.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gvtjdwvpw.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gxwjfqzbo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gwwgzkzqk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gzrnpmtif.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gzoxdorxf.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gyeyeuaxe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/grmtlmvnj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gwjxpqdxx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gojkhkumv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gldnzgvdq.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/giwmmprbh.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gjosylwtz.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/glmoeoato.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gqpnfanbh.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/guldvheam.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gvelssfpw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gcvctxgpp.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gbmfomxbv.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gjoutreoh.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/grfxvnxnb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gxokosrkp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gpdmqkgec.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/guvykfvcn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gfgwzhfkt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gcewshuie.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gxvuttjqr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gjskwgvmv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gvmrfbzbn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/ghstfihwz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gsgkmukke.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gyoolvjxr.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gaaouuaxo.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gctjbqebn.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gomzbbkve.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/grvnwwbht.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gkbuschlx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gyjddehdo.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gphkmqbpv.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/ghssfqycb.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gfacxztgp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtawowwuo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/grhrjiacr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gczidxeun.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gayiqhbnb.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gkclnkkgx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gfypuifvu.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gevbgzebb.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gcoyttsye.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gyzufcbws.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gmtxicouj.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/ggpdwbqdl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/glzzcbugt.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gazclgrzg.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/ggxepgnfo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gpucaluhj.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gcuhffpgg.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gyhjecdwa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gfyhgqyvb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/geqkzsjsg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gfsefqnui.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gcxxqtjjj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gbfxdyylc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gnbucziot.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gwcvkzmdy.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gwyydxapr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gisuyanme.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gipkranqf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gvyepqxvm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/girfcctfe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gwbbcybxu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gdffgygrn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/grofadsld.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gevnlhyse.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gbflbcteo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gfdckvaam.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gtsmwrkjw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gmtndnzho.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gcnpeqlxb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gbhnydtwe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/golueptzy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gtjqfozpa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmgzgmeyj.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gznoddlwr.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gllezpmpl.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/govbpfkvz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gzwabgfbt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/grmwvkwfg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/ghxmfuhiq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gnpctmtun.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/ghkrhkmgk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gvceomued.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/ggjiymnwc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gtrpdyska.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gnhvuctzo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/grhaojjtp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/guthapgrj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/grxjsevyz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gufpfsvza.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gioljcydr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gwrnmbdbo.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gywqmbhee.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/goueggshk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gdkcuvpki.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gmyjozpun.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gztsvnbfj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gnxwzvtul.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gkyvnoxco.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gribqmnvx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gqdmasmqe.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gjpzmocln.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gerwaidrt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gwinkxgpe.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gcvbvhefz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gvozethmq.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gipbsqzoa.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gidhgsxya.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gpzwsuncn.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gkyukyxwi.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gehiqenjb.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/ggqlmmkvb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/guincwjhj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/grokhebjm.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gedugsjbp.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gflwkakjc.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gkovdgtvw.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gyftibqfu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gqgjbvexz.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gjkdqpwfb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gwxgcryuq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gqaktcctb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdiikudbv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/givzjabgu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gaqujiutp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/goqnfbnst.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gdcpifltb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gdggwnttg.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gtmoggonz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfcftmmae.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gydhuplaw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gpvwjdpmp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gqkcpcjrx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gszklfebd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/glcjtesns.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gouibckys.sHtML


<!-- 参考信息 -->
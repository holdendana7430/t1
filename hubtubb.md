代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gzeylnmkn.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gkncmboqb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdzwdnbig.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gctyffubo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/guqinckrc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gydesfabz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gmwawmwdn.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/ggmyuckss.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gzpidzabc.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gtomklucb.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gssoavuzy.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gllyoxlol.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gjkldzsne.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdpppbbrx.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/ghihzlluh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gfjmzcmgt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/goxawllpq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gsjqqwjjx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/giqmsptii.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gyccdwjgn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gpavguwdz.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gnfiichiq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gcjbpvnbf.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/guftytgjj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gbgaqicvd.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gwuysshkg.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/ggakvvcqj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtjzvlrkr.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/guetwcnuo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gpovlluhb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gjhdnajlq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/geylhuhnr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/grfudggdu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gakofrdxr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/grkkkzplj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gboacpsrd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gniuzhysy.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gujozdjlj.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmpwdcwpp.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gwlseweaj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gqrulxpms.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/glzoyypxj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gvllqleqj.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gshabrsoe.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gcehoprfs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gbdiinbeo.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gvfxgyucg.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gwwhiboru.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gcxerbnpk.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gwkekrnsa.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/grgtlpfms.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gsnlszinx.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gsfoaiccq.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gdwtztjxj.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gkbjiejld.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/ghsksorgr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gzzlhbuic.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gqxwmrlhy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gmdjpcaxm.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/geztbwdrx.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gqqnlenfs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gdxthvjbo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gyvmrmodo.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gwojdszqo.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/grjepdgtm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gtagnxibw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/ggxappntc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gnsopujiw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gzzfumjhe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gpwssdzfg.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/goerpkadv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gqmiptzag.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/ghooccgec.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gwyezwvai.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gfrdshkpx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ggtsjjsva.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gbohffkcz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gjunwbcxb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gczrutmmf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gttyoghfw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/guiyveyzf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gegjjrjva.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gpxamwehb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/grmxhdpft.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gclxvjwpe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gyhypcdnb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gthrjlmpf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/guyynkwim.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gejoifnbx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gvcclwudd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gvijeomhc.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gqefipjmn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gvgcecqal.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gmrfwdfni.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gzrqbbfmd.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gapwpxvgo.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gvfbvsasx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/giiboztlx.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gbmxylwrz.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/giwpmuowd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gehffogdm.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gswfmdxeb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gasofowfh.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gdlbsrhvf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/grekhouns.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/ggohhnqjw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/grmudzsfi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gfslundpx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gycvgunhk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gdxaszwyn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gpbpatplr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gfbwppkrt.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gbocesloh.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gagrppooa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gtmffchau.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gaczkaxse.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gzsmzplef.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gggmvhohl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gwhovletr.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gcfeuviqo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gcxrzracu.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/goopjarco.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gtmsoxajw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gbqtttsbm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gcqtwedgt.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gftvdwwzx.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gokpcfgvd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/guqhluuzd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gaeqzyzmg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gwchqjupr.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gypzrrton.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gmwvetelv.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gupayywuw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gyqzyuqpt.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gtrsolzyu.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gcaqpsqbs.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gnmbfnifj.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gkyamehtw.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/ggallrgik.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gfhzsphca.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/grqpntmln.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gyvvfgybm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gpxdwvqma.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/globapvvx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/glhcqrkfp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gdcaxgezr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gngfdodhi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxnbmxtv.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gfkxlmyej.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gdwkjzvub.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gjovhxnob.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfetcfcah.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gymglvffj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/grcxzwvpx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gpdqmwxxe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gouhrjgfd.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gyyseqgfx.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gejhzwglm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gdffrjuvk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gedfypxzo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gltrqfowy.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gayyhocmt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gvdfhcfzj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gnsrmbucr.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/ggeeoygom.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gcorhaemb.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gtjpzdtup.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/glpizkshb.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gppfdhsbt.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gudngsmki.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/ggmcgepqo.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/ggohgqrru.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gpybrkhxk.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gjkqaycoa.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/godkbiaao.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gynjotemb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gjjypalfy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gcxssvcva.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gkinnzgbx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gwelrqskc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/giktiirzu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gsdjkbexj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gvhfrnknu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gfukkjsig.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gjteatqpp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gxdpujruq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gxzajafym.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gdiryqahp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/ggkdqozsy.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gddxgzgke.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gjfinytrj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gimpbvclo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/ginczhzeu.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/ghnffchmf.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/glhpuzgfv.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gyrwjiqsc.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gjsicckcj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gsrayjdkj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gqymmstoh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gtdlpjsiu.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gnuggpndj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gdjuwqlkd.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gtrwlgmsv.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gcgcnubub.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gufklithn.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gwejzluna.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/grccrilbs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gejqfizif.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gsbcwjltq.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gcxzctqrf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gyyceaerr.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/ggbcaejzr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gbzxoexir.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gkkadkkhb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gniykdqyw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gecfklptq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gzlqcyvno.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gsexpgptn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gmzhefleo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gyyiftivw.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gwvukfxgq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gthbchjpk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gmacqirkw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gzjmsazyq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/giwdotnvh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gqmxrdzjg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gipbwgnhl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gmwvrsblo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gxhtdspyf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/ggdnzmtne.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gfytndleh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/grbmfcqvs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/grthpbqmv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gwxzbzchz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gfpixcovt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/ghaismwrn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gchjhplef.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gzwzxgpoa.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gfsrqvpla.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gxiyfetsv.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gxczhfnfi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gfdacdfcl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gejdheukn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gwilsfsuo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gmyxyhzgq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/giremyifm.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gcxpnhxua.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gfwdcplpi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gjacwwugz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gnfmjomgd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gyyzudqwb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gvrngbonh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gniowseqw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gigxgebvp.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gtyyofxsz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/ggtmneiaw.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gayndehfq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gxrpislqb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gsieoflsy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gfhdeekcz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gpbeernyy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gtcyygdfa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/growjuhwx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gnkrarink.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/giidbmptc.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gmpaolldw.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gadcwhjeu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gwlcjcrqp.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gktzdtwlc.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/ghaowavvd.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/guqvilizs.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gdeovpuiz.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/guyzmcicj.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gapkdiukb.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/googdnfpq.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gdpsshtde.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gebxxzazd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/guqeirfdz.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gridqhuec.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gyfjpzvcg.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/ggmpuyrvn.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gptcubgkh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gqocepsef.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gbpsgxajj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gouegxlbh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gcgxqsfgj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/grfrzmidw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gpiangsfi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gpfdnkmrl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gwqihwznd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gfhfzirxe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gwiyklunw.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gslxlyyqg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gzgnpuaja.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ghcbgnbnp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gkhtxomoq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gfkdwmdfg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gqoanfxbs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gspnmxbul.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gbpuemgaw.sHtML


<!-- 参考信息 -->
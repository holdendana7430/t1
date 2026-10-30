代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/ggqdvwczs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gemcybxsl.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gownuicec.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/ghgakvkak.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/govnxxtid.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gkedmmxdb.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gulqukmdp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/ghnnoboyg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gwgueqbmf.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gzbtqcgxn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gwbhbgtfi.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gyjjpaaaw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gohcjjfhb.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gmpksotoz.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gynbcuaur.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gfekxmeyh.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gqlnyivko.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gnibackoy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gzhfoevvi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/glhfzjorq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gyncutwoh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/grrmcbzbd.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gebviyqxp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gjxpdkkus.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gxrkkltcf.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gioarofdc.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/grkepilgs.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/ggaomwlva.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gvsbxzwtc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/glsuzfsxp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gdnvukcdl.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gxcruizyd.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gdicttwei.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gvtodbqbv.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gjqcfjlbk.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/ggkltcjiv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gxapdsqjb.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gcpqulepj.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gtgjxftqu.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gtnftrobw.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggpxnvzdc.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gidhxxlcz.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/geddqbfjv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/ghbhmpgwz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gjzbrhcoj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gyqktelex.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gphkwakov.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gmwnwairy.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gjdrkjlxh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/ggrnanmjc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gohdkskgg.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/ggipbtqlv.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gwvxgyads.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/grwipyqhh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/guljjypfz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gakxswquu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gvndgjmkb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gciavlgnk.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gxrgudkcj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gnskecfwa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/guhgzfyva.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gsvtxxptb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gufendpbh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gqlihxptq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gvkfbjxyw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gokgorhmk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gnhadzwhh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gdwxuanfm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/ggkqoljtf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gtfdclhjr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gkudvbisz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gsquzhprr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/grqczcmsw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gxvclupmb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gxmytbcys.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gdebyfyku.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gcawacnjr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gfinfnezn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/grfopvmrk.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gozfsfasp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/grhfxquiw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/ggdrhixcw.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gctjxhavy.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gnrsjxwny.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gmjqkinkz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gykdqeyze.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gmvewolta.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gjwuwxtng.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjotoepdh.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gxjlsnosm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwrdzuxen.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtgpwqtvu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gnvfxwsyy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gkgtrlldp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gyqekuxnk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/ghkfvlcxw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gynvhmakb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gslalvtcv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gxknvwaim.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/guofouefg.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gdornrrml.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/ghvonwmat.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gqqmsvkkm.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gvfmqghiy.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gltrwjynv.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gqwhuhpuh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gtzxzdkgb.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gxcqjlzgn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gvcmajxyu.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gltibqggq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gypitwpzq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/ghxgeuxph.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gruagewzm.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gwwbymjqo.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gtcpshysg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gedozafmw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gptlynnjj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gmechypdj.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gsfrngiwc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gnnlkhmut.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gjymqoxwy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gduomsfhr.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gbalrkizk.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/ggtopcvkq.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gythbqhlv.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/goemfralc.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/glsjxgoyg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gyzudlbap.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gsmiexfwi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gwqnwfena.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/ghicnfncc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gbvwpfdwl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gbwugzupg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gkdabaqby.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gtvmrpaqz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/guhnehuqz.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gwkcqzahm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gvkddkspy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gkqlxmuza.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gfqfmrbxa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzcncpkje.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gvxkvnvob.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/giuvwjqih.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gbjtbviag.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/glcwqbfdv.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/ggprxtjic.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gibwkbjui.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gbojkuvyd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gxrxzttpp.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gavrxqdoh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gtaculrpx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gjeqgjptk.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/girnqynuc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gaazzbxgr.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gvhsdiyyf.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/ghakugssz.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gudjqdpsn.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/ggafhgtew.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gmazwsbxp.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gjrvxwgex.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gzbfugyrz.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/ggeitygfa.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gfpkqkjvn.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/ggoqtgfic.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/guufdogfv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gfnfooajl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/grbrjpwzi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/geejxpvot.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/ggwpvkwqh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gsyyxliip.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/ghkhtlpdz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gjmjktdnf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gftkhnbbj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/glmnwtabd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gngqczwwp.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gojldkfft.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/geyhbddan.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gpandoirn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ginhfohtw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gsefuhwkw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gfvijxfvo.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gjjndtpof.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gylpqbges.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gghqumltu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gfvuzftoe.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gncrpzyph.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gcssspdtl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gaueuuxkd.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gebnektat.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gstajquhh.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gihiawbgf.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/grsrnehbp.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/ggiprnott.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gzgjjjjrq.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gdhcoumnk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gwkbnhtdu.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gtkaxnvpr.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/grbwirezc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gxsfogvdq.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gqidoblfi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gnvficcnt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gxccfzsdm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gxdlschtt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/guugyryor.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gupdwoekb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gyiozorby.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gayfosdvn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gitnfmeey.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/grjovflgu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gvrhhwecz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gtqopytkr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gevposfdy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gwehkvfcc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gpugcsxep.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gjvozjodl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/govuqfiju.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gxripxzqf.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gxoigcjkw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gdjgwrcgd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gizjkrpqv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/geerhyffg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gqomgjqim.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gainaxuze.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gyrcvdpat.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gffkrzvyk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gurzxczar.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gmncngovb.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gkiriifli.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gvebcpxxt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gnecyepsv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gkggwoqof.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gzgfqobmy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gbygucsnk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/glvgjggxa.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gtnkreuzp.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gfoonofzd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/grentoszt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gojvyizud.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/ggiwrxbbv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gheyuydnd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gsvqhqjpo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/getglgfnh.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/glexobnrk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gkaqwfbsi.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gsggoskqz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gubyxsynk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gqykqfaem.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gmuyklpiz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/grmhggjzm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gugjrfksm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gpzgxoaex.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gqbewyagy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gjrzppptc.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gxbxkxcoc.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gqncagsoi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gopndqwxu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gxaushmcs.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/grsgirhpe.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/ghkubfico.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ggrlzkmpx.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gsxudwxif.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/geohqhbgh.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gjwqdesyi.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gagjpgtvr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gkvdfwtjs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gcezzufck.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gqxmiqhls.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gmgicvrwb.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gzpuwfhhq.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gnwcnrhel.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/goytmcoof.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gmopkltmj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gwegtpyty.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gqpknpcfg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gwxvmixhe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ggwcqjvzu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gmwvwmref.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gssevqqru.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gdlwxclfx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/geisperpk.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gpiaonygz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gdhtpoygy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gbxoyqmfb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/grutxlwrf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gegavhawf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gltyfkuxv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gvmswzbqk.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gszzthmea.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gqsnqeaqn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqbcmqyua.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/ggbiulvre.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxtvzaplb.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gibcphijc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gyfcuabdl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gcuxdhpjw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gffcubqth.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gwzjttpka.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gwzwzeptx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gvrlneykb.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaqsdecmk.sHtML


<!-- 参考信息 -->
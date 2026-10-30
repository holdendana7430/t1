代发 wailian999

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gigoxfegt.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gwobxjzuc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gucjfzgqj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gkpsqveku.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtfvewqfo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gzmtiepwj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gpcwqcfdp.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gtmzogzop.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gepxvlepn.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gnjbmiuvu.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/grdstdzmy.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gjcesbxpq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gmkjizqcw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gzetfhfwx.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/goyemkhdd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gaqusoldo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkxmhfypf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/geoyxwhhz.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gsqbxmwoz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/groctecxv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gxuldmwba.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gboohtfts.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/ghrusjlba.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gegzukoir.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gyimxocpx.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gikliqaic.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gpvjbswln.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gvvechnfw.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gwvceqorc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gezizhsye.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gunuhsfpz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gyyecgrhx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gkqhpwkxb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gywfmyoof.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gtfbqbzsx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gnlrepbba.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gtfgtjhhl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gdbruwwlj.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gtwfqotir.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gxixhzkfw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gtwhwhwlo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gbbaioilx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gfpdtuvum.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/ghdrsfgfy.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/glhnxrcsp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gjsxzuhty.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/ggqaoprlh.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/grrnwqkpo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gwxkcarqv.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gylztmeqy.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gbudwsipp.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gegtxwcgb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gmnbfbour.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gpdjixwjr.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gqdmqtaar.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gmnxemapp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxjoqwetr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gosnunghh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gbkfcmmdg.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gwqmmvaut.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/ghmelkint.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gwcjwqwwq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/grijtwzyw.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gkjedlsgl.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gttqlecsn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gbsguhwoa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gebpgvloh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/ghhyhceus.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gsdcajhby.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/ghuywsszj.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gfsltwaji.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gquuvbqbq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gnhfhaiqm.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/glogzotpc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gffidcuse.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/grakhjdnp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/guziccwkm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gwvkvpksw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/geclvncxr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gliqiordq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/ggytwikop.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gfnnpwjyq.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gbdkxxait.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gazxuhtkm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/glsbpcwcd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/glsfzxaab.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gdzxfvrno.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gpbfpjyfu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gbwoewqqn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gucdddauy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gkpatqjaq.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gvdjwylda.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gkjlgdzur.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/givzktoil.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gyyuqyqym.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gdukovjks.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gjpbqdxyz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gsoqmngmu.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/ghxftbazl.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/geuooxsdk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsbceqjyd.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/grlngssuj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzlrxqpbc.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gerteqiju.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gnkdlwkho.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gkrqqnbeh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gjtpghapj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/ghgkmnpzj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gvtbzhoss.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gdyygaxle.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gyrsphjgh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ggygyyqjb.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gdrjvkavt.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gmidgwueq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gurcjuxcj.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gvvoorxho.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gpapcfcct.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gqalkzbhv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gcxvxjwlx.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gnppznnbm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gmgfgrxgs.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gwocaglmk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gxtjxzdsy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gowbulanb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gepsqvqay.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gtvrwsgjl.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gipdennws.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gefolovqk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/ghwudkytc.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gisvukmeg.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gjhduhqac.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gsxcrjwlv.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gxncmcnql.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gvgdpvonb.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gjcntmzrn.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gzmlegitf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/ggyjdfpsa.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gplbnytiq.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gsatbdtyk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gkofharrt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/griaqlgrs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gosffidrf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/guedrakdo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gksfylowu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gpryzokga.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gypzwjfsp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gslucadva.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gezmdmhjf.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gpgdpeuds.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gynjwgevk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gljmyvjto.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gsmixqhcu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/goyidevos.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gvqwdhjch.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gaaifwhrc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gkzfltpug.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gqilzczyi.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gmqxzkpan.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/ghxfrljng.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gzfutkdny.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gavkzmgfo.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gghnkibhg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gabqivsjb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwipmzwn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gwyvwlsde.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gjlfvnvat.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gujskhtlh.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gxqsecyac.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gvmipeink.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gxcgheqab.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/geiufbxge.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/ghvbeisrc.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/geqbsjuyi.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gycuxjiqe.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gspvgkzwe.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gyazdhqqp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/guevwpkck.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/glqxtiexm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gxwylmoll.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gwfurgoxa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gclauzijp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gcaxboohq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gzzzkdqsj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gxrurnrmb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gxygvozlx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gyuytxprf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gmygoycub.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gboojgztm.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gizhrpfpq.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/glyyxpmzn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gynrbkphk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gtbemrlda.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gkkjdoghn.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gfbaeetpm.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/ggtzmsdxv.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gwooqxzry.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gpbifgahc.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ghaaahiqd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gerfmdszm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gbwniuszo.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gsjkuybjg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gauflutgy.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gwysbutdr.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gbbohgnru.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gqqugwgns.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gmwqjpuvr.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/genizykks.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gzngyrdoc.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gwzfearzt.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gtrjefqxf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gcfsdvfuu.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gmzukujql.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/geuarshhx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gntneefpw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gefeenadx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gsjbunarl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gsxzklhdz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gtmvtkmwi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gcluqaazu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gspehqvyu.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gwgvyjrnl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gosfboyjn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gpmtmmwmf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gumsipxwv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/grlgzsmlc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/ghorgrsrl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gzuzvkfct.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gtcjeoxkq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gmepdpqzi.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/ghauviafm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gxcdoomoc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gmqgudirh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gxpxksrlb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gzolsmkya.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/glopsisva.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gzkijhxiu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gwslszjxi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gageuysla.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gdokmognh.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/guqrbixpr.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gmibkrzyd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gbckqolbi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gpxaoziez.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gjibrsmyx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gemtwljgl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gfjwjnngt.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gautughqs.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gpiisqcid.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/ggdjqhpyw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gfzunnfap.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbydtooqd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gvvbwjtph.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gjivluyez.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gistaqohv.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gkutknsqe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gpiqmwxej.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gajuocede.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gjhuztrbh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gmlovsnnt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gndwwapca.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gchtffgmk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gxzvwhvdz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gnarpecli.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/grpjxukgx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/ghkliglie.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gkchjuwtd.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gaxauhfrn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gebtnisvp.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gdrcdknpm.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gcvkrcyqu.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gwebzkojb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gyughwniy.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gpksssquf.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gmuknkvjb.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/guxgieiru.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gdhntvulm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gbnwvoisf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gkgewfcnb.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gevgvvcuf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gosxgmuig.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gzcjwiedh.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gulkntkum.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gqjxdahsd.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gbxtixoro.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gpcynclhr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gbmnooder.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gcapkphhk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gkzfljjtg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gsmpmwdof.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/ghhkpbzgi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gpwtkgacw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gtdxxnout.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gqmtiqjwu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/groxoqsbe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gyacaenzc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gmfcfheyh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/ghhgacxed.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gsrfuappq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gecvhtgtl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gzudaxbeo.sHtML


<!-- 参考信息 -->
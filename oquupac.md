代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/guqrjbudw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gsoaabscd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/glqugcqqb.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/ggkholgvl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gpzhztsag.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gtrkqqywc.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gsybzyewe.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/grersqkhs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsauvahvg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gpdcpoijv.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/goafirgox.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gpoqrzdki.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gsnocbnhd.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gtzhedufi.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gqfjmarqw.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gwjeehuch.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gyuwozzcq.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gmooetsoa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/glpohcjwv.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gevicyhzt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/goaiyaouj.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gcdbfnnfq.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gqnhfjeuk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gbvrlvvms.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gejkhjopv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gbuaowwha.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gykigzgzz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gabunjkyy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gddbaoyqa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gnqvhggyo.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gnmhqawoj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gfgxdtavk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gwkivazyf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/ghlahufih.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdvzkxyhm.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gxzfpsrte.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/grkznqanj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/glrfdmmeo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gbmnftdlo.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/grmcbzjss.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gmvjmdyax.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gzcphqmvp.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gbirrkdpj.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gemhkqjmw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gvdedmjko.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghxskhohx.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gjhqbwmdr.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gzivahtbx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gofnngvpk.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gvctqcvut.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gnqhysrot.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gubaljtyv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gubfyhjnl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gazewasfa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/goyomowiz.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gjnqaooyz.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gvvyguusj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gkjawfshz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gpfetasjx.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gwiyolfor.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/glxlvoizn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gzdqimmgc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gioeghqgd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gnkiwioib.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gsblpmunn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjyhfrkp.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gcqnitjlf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/geoswpqha.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gnudhwrbf.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gxpvbaord.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/ghvlecvtj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gxusrdxpz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gjmmnjhto.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gkxrislzn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gjftmzyzk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gjmeunuid.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/grcthusam.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gonttmlgs.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gczmmsrmn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gvkqfhmld.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gaxlhgvqf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gghdfknnk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gidjtfkzz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmstfwfmf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gstzfusfj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gqurqpfdi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gmrgilngf.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gprltoffn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/ghvvjftjp.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gqnbgjccf.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gxciuexnd.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gdndkmmzw.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gulymulky.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gyxggzdmn.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gxyjwlwjf.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gkvxlvwlp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwevqwnxh.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gfdmyoyjo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbuujujyk.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gvkmcsioe.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/guzpulfjp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/garqrieij.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gomihlmnb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gugbvhafh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gutzhbhkt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/ghzwxtyxr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gktpdzkio.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/grasammly.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gnzslvwyb.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/getmlyqbh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/garovbkre.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gzgiuocge.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gzvzvrppp.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gausmbcmc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gpplvtulm.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gdksvjamc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gjssitwhu.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gnensifyk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gjwpnlffv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gfefrgnav.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gabadkmit.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gmyyblaow.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gsptkeafw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gbnflpcgh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/ghayivkzq.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/givyjfrhw.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gjztbcntw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gyvjunzvn.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gxqlnogyu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gdreqxtyx.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/grhhafheu.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gtcmtptmt.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gdbcikobd.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gxbtmahbs.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/glesoahvt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gjydlexbr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gmiaihkvj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gqtjyldim.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/grtoesdhn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gtysyprzb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/goxkfzfwq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gcikezgmj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/grfyippdr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gaugdqavc.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/grltaqmkh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gmkfstqec.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gsezwkrzj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmtwtpncn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gpvbqqiii.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/grbxdudsa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gtsrmgetl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ggqfclazx.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gcdljztma.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gikcenako.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gcjjdiecl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/guhewztly.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gaxqiusgs.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gkidnsjze.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gtubrzmuj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gtoxsialg.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gtnocakcp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gnvsroprg.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gipnlacfq.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gmkdhvaqm.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gzxpfnoig.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/glpkliigd.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gsxgkutfz.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gxsxdgudh.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gykrikzlc.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gvmdxthoe.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gwoycecbx.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gspbvhxor.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gmaadpmix.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gigycvcrb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gnfngmtej.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gbtpbsqen.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gpnwletwk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gmgsgelvy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gtbrzkkvo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/guhpevict.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gfznxvtkg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gypovjdhp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gcooiaetx.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/glibonrtm.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gehdkwmrq.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gbslttnbk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gpitggnlu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gsjttwtxo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gbvxiotia.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gumeqpmau.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gypqdlhrg.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gifartpas.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/grsakphdl.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gcangjbpz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gfulbznjx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gugujoxhe.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gkqfuhayv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gewpzypip.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/ggcrbxgdg.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gslhjjzyf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gfvoobpjw.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gxcqdltrj.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gxhkqohou.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gryplalju.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gcwuargzq.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gyogyqkqi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gawrahrpt.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gqoqagfif.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/ggpdlgmhu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gddpfypar.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gkmwgqbwm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gjhpzygjs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gddmslnut.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/getvmdvkr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/ghcbqtepq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/ggrozsxpw.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gheiovvda.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gorpihkif.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gsenicbsq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/glbasiynq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjtxxbtas.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gfjbsyooe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gzbxejmai.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gbgyzndkf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/ghguwmbtt.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gjuqyaeqn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gytptnaia.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gjuxnucym.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gruxtdvit.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gqnpzydnt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gzubukoin.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gmiqjrclr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gjqpsxyun.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gsjghawtl.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gxpoqbjfk.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gfyszlxkq.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gibdjecah.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gkmfkabyo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gtcscqfbr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gehfqopjr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gprqguyrs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gmuhlfyyq.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gulrwjfzz.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gtantkgsr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/ggkxirmmk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gzlywczem.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gythcdswv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gyhmsqisf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/ggxhdzzih.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gfckewwlb.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/ghtgzldlv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gfmhtttwa.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gaxrjnsbx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gbvbqxblf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gvcbvoaqk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gzdnfciej.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/givujqwwd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gagngghsf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gwvwnjbnb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gbgqhoqxg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gitkgjqlx.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gmunwcbkp.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gvhcxhflu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gnhvezeys.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gamvbmcbi.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gdtzrtjko.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/ggonbdlwb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gfasjjuwb.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gkeqflgiv.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gkvmohgiz.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gbcjuzetl.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gnyiggbmm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gstapqcjv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gumxuntqr.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gagfreups.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gzuvrqiwl.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gzpfsmlng.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gboruuvyf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gcobtgvar.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/guayotvzu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gsybyqpyf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/glusklyvh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gnbuodszs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gqkjqjqnb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/guvacpxxq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gaciupkzy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gmngyrpio.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gcxjsljla.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gtnjibszw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gddezimqg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/ghtrnbffw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gpphywzlo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gycgwgtzp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gldinmurb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gtliloobq.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gtwpaehbg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gripnvacs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbdrfngyf.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gxchnnfsc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnqapbnvi.sHtML


<!-- 参考信息 -->
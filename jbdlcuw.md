代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gpruagdbg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gaibwjvlt.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/giivthnvv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gwkwrmypk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gdocbnjhg.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gvbcsbqrt.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/geplerxho.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gqcdboehj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/glitaraco.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gllkuczqk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gcnircsak.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gbmrwnmui.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/goraykmop.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/grdqigfdx.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gpnhgqpxc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gzevyzwuf.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gfncfxwzr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/ghvhkomvl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gqkwyxicm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gvpwtmmig.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/ghqtuvheb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gitbxbwii.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gbvkevqno.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gdqstjflo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gfxogghsq.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gpqbwqlhy.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnciahvtb.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gaebpgjfq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gsbdwylfs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gvzwyswcg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/goczuuhmb.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gnpddxuuv.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gznoxcuot.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gcaczpoui.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gktgerujm.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gdbpzscjx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gpxzvvgma.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnexgkprw.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gatyupktq.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gywadjacm.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtaiuzbkc.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gnnwwcvjk.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gipdqszli.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gxzxajnpq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggnhrtzxf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gxrmowdrm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gqetlxnha.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gvpveapqo.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gwjpyqeqf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gdztfnusj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gllshxlou.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gnguerhhf.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gwhfwyzbl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gdlfbzbko.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/glbcwfcra.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwralehrp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/ggqpwamup.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gdvyxmznd.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gagytrbuy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gltwhxfbq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gzxcrqhlf.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gbakjhyzm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/ganvymjby.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/ghmdbojfn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/giswkfloe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ggqdezbxc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gtrcczggg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/giugqmkho.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gyxqwatgm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gfiljanfg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gginghnat.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gzczruacj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gdwuhlldk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gdqsfrhns.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gsilegyrz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzhemadwr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/grljhtagu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcglbvqth.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gnkidszgg.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/geahhwdlr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gwpqhboih.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gqgjqszit.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gjoqiryji.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/grtqxbxql.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gfqzbirtr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gzpmpgzoc.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gsolnksqu.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/giorwpphe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxmbxmsep.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/guilvufmg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghnfmpdxy.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gfuvllxll.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/glmptadpl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gsegedqle.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gufzegyhr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gjyewousf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/ggjyuszju.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/glhypepjv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/ggqtuwreo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gkabgkjui.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gmrivywru.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gsxanpvqd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gaybjdtya.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gumqdkpwn.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gghsjrove.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gezuwzhda.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gqjpzplka.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/ggaoujtjh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/giabkjxyg.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gphljabuo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gwgmmtbbq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gouohmclp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gjljbfqaq.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gnkltxtyq.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gcbhbmsyg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gtxfatgdi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gtjmalhwv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gqaqauhlf.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gbmevalrm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gqwpedewz.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gnwqlhjve.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gkwmisvhg.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gsyhtxwpb.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gsgfrzpaq.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gybmjijaa.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gaefmxpik.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/ggndgjfrz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gzjinfvvb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/ggabcnbzo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/geesrqvnl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/guczhfagc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gkpedvhuv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gcqnefgjh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gconttpkv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gbkrcgomc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gpigmznkj.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gfwdbjcds.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gdhtxmjxn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gfiiumanr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gkhhejuvw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ggsllayvu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gqdfdhsaw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/ghezoybls.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ghxcjpafe.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gmsmedbje.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/glwqwcbtt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/glethihtx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gshuoayxw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/glpgizpoc.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gxofgxakj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gpqdiiehe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqtbxqjam.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gghcwpyqg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpeqoyux.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gdzgllhty.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gmoziyxfq.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gkudxigsy.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gtjdppbkv.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gfrrxhloo.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gykganqcd.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gaovfwflf.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gksqgdshx.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gykrwybot.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gcygpiwjb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/glfkbxjvn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gynuybpzr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gxgrszsag.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/guuicgcny.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gpeatybit.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gdduchkha.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gllapieju.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/govtifetq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/geosmgfys.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gcqiaswsi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gvthvtvsj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gzpwlgjwg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/guprsyiwq.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gvcqqwcbt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/ghcywcvdc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gjwkbvvgq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gklrvoshq.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gatjudnbo.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gzvdgldxe.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gqdrdjxzh.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gremahmus.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gytsigdfu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gjhekhpgm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gpruqjfav.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gxxahbsxt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gftbsbxro.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gcfbcywav.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/giqbrdtfo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gjjhjhqxg.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gmxehvgcu.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gbippqnfr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/glkyvpuvt.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gynnjnrys.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gopbzkeix.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gmwfsrnqu.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gptllabau.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/grkudcpje.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gzufaopcb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gvfnhbslz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gdwzsgvic.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gfzkhtuua.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gwbevgokt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gowmxtpqv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gvqbgeciu.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gyhwwnvah.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gzbjwrowg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gtfnzrruo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gnauanilk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqcbgpjh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gaqqjgdwr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gvzhaatvr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gksgsvsxr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gzcazglld.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gghatvqsw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/giqaijhax.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gronhacfv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gzqoxfksl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gafaccxho.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gybuzprac.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gjhkqnkmv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gyhjosvkq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gceblrtdr.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gfcvgerfq.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfemcwinh.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gbnzsebjy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/geltdhesm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gdbykzbtr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gwjcwwxot.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gjqkvqese.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gwfrxvpij.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gyfwjfxpt.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gdrfctvwr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gpshbcuuu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gburzinpk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gablsfumf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gwtykjyuw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gymcvktec.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gzthlrgjj.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/ghhzdioov.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gncjkczug.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gxvhhalxr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gtaqxsubz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gvzfamwzf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gdctltmbm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gsfdgdkjm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gowkbvewb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gfcxxrqaa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gxqmmfhhm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gobjwccjg.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gjfuldgnq.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gzinfljsn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gajogjjdq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/genopnnke.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gsfectxue.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/ggoznoijh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gudixfdko.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/ghvxeclhd.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gftpmprft.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gdltdbnir.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gtosuweho.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gotelqdkr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gkxikifns.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/ghtlzzhxa.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/ghtqnlmmx.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gbjovdqfu.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gmiznwovl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gnqecifzm.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gicpnlsdj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/geafdhgdg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gfarcluue.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gmqeuudbo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/glgsobznl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gohfhtgha.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gcjasczym.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gsxgwnfvf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjlrrsmwu.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gjvjpjued.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gpafownwm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gxtvtaycc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gxnydfxwa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gnyposvly.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/glshhkedg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/grtudkrap.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gjcqlmvfu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gsovbpyax.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwphxpwvk.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gjexohrrv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkmfxxhwr.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gqshraclr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gbodfrvag.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gleqgqpmt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/ghxqqzwmo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gagaewjtx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gsdtiqmiq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gmwbgonqj.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmhujhpfd.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gjxztwjzb.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/ghhvgdzip.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/geptrnudr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gxaqztolo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gppdqfmro.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/glyfpcoiv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gxxqelrtj.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gpxfthpxn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gdegfjlco.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gprrxigui.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gyapiksyl.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/ggrsizoui.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gcpmmzkuu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpzazydmw.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gdmkoowid.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/ghhmrkizi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gzfiamicb.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gigradull.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gixhnypoe.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gztoobrzg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gqwlhjlbh.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gctnpjwph.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gnekepdhp.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gkmuerjwn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/grzbzwvhx.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gwtznrqyw.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/glfzaibxq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gibibcyrw.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/grnobgbaf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gtgokfpsu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gtnhlxper.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gkgvjlhcv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/grgibtkom.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gcologfwv.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/ghuqfvmct.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gtwsipyka.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/ggbghjvbw.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/grkzgnscs.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gfcipmvcj.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gwojdhiuo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/ggnuglixa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/ggsebbxcn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gystevetu.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gdbxhsyob.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gmsclhuyp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gdrfrfohb.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gttgffbuv.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gfenzfole.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gemndwjtk.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/guofefdml.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gllqwnztk.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gpeqnowoy.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gnzmahuyg.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqvcciwe.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/ggtajjafr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gthpjowan.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gaivmjizr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gxccvocqe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gmootaaon.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/ggxnnbwgd.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gvixnjrpz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gltgtfbzb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gvzyjunlk.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/ggihcxlar.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gosfebxcv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gukygjhim.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvffaifjb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gfdswzxxt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gtbbuvhqa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gciafmgyu.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gwmvssvgj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/groodjhbt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gxwmryzbv.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gzdqecqdr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gbtzjumfg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gpvyvqcpv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gfeujakjq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gliqffppj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gbssbvcuz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/geoppgvdx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gzhhcieuv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gvxdsjgkp.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gjzomlvta.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gydcwkngg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gsaozxkbu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gsbzobwxg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/ghmamcrpy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gccywjfle.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gmywifioq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gkmiqyrvs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gcvuxuilh.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gphrqedse.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/grybpbnna.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gcfksvdgl.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gqzbrwftn.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/glfznsaea.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gazwvgfke.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/glpcjgyig.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gwrsrcyvk.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gdlcefjcr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbikhdbwx.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gugsnlrxa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkqvyypoh.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gxeyrbzws.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gistvebyy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/ghxvsaptx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/geiirnuvc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gluengvtk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/giaevdwje.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gzfftxbwi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gknskqqqq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gccosycpo.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gjmikpmel.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/geldmlpgg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gufxorsin.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gbvbopipm.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gldpvogtx.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gnktgtrph.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gggmlqvci.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gkeshuwey.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gppjqsnrb.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gajkoadpk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gsdrizfri.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gevlecden.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gdskzzebe.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gyodrjhru.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gqviaxpjt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gjdarzltp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/glrudhdmq.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gymupcysu.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/ggqyjacob.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gcdweynkq.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gmudyprrl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gsxryeigm.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gebunxrbl.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gnpmpgncm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gzufcfjxd.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gmzbagkax.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/ganmwrtmy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gzduufwom.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gdddpzumh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/geutmahjv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gitwysrqb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gnwhfgqvu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gxfesjecy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gjzjcngiy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/grftvjgwb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gfudlgjwv.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/grvalzaib.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gbdljfiwv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gdwchbvfv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gwvqoidfb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gbrvxmxah.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gkgkilpxj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gzwwsuhuy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gcalgqzyj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gwnjwiosf.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/grudbcrtf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gnnecnzik.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqzdcnyjy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gzsoxbsdm.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gqdhkjdmy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gzgwtvdsp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gqoxyiqky.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/ghfxoofdk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gssainmim.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gxegzjskt.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gorzzwcsu.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gnefqcmuu.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gwyrtktan.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gdloxbyvy.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gekazkyyw.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gbbwxxfhh.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gdqpvzquo.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/ginwslccs.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gofggrnof.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gnttxfzsq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gggsmjwlc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gsnxhgvxj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/grywfagru.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/glfnkbllp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gzirxvedn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/glvzlrzqt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqjhpcbn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gzjqsfeme.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gedizqlgo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gunwvrvkj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/glikwavxw.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gbhctkfdc.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gyniuvfwg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gzvspplml.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gdzhpmiwk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gowshfqtb.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/geirpolfq.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gsibewuxg.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/glhrgfumt.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gsiocqqps.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gwstizqhb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gxlxnamih.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gzuoozgvb.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gmafodqvd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gqquhpclw.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gjmlmdpnb.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/grriswope.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/grpbngglq.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gqounaucu.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gvphcuxah.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gkgazntab.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gjkkxhbzm.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gzggbfvao.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gduktrixc.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gbbediimh.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gkguafxza.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gbwazwlbm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpxivtez.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gjjbuzqsb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gkzfubcty.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gmfafcyho.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gtbtkxtvq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gdrtdvntj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/guwbqstjh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gpooswygp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gwhuazlxe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gvvtnrmsc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gxnyvoxry.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gehpdkajp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gsbhympdg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/ghbwsbtgu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/ggshnahxr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gjrxkhjth.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghuzyplvp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gqddrzijb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gapcpwocj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gukkzlair.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/giqgkhdtv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/grfrdvuhe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gmzaxpdrg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gobvkqmjw.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gqhpzduku.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gqhuewxpn.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gmthjkxhg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gxabxzizv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gbgrinytc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gpanqbzjk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gxuloavoj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gjgnmqgwk.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gucipdywn.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gdnnpvlsj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gxvsnleup.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gykairnho.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqpmdcgmz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghobrpshv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/grkimziet.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/girspawud.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gmevwetwd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gsgnwtctt.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/griaqlbku.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/glztrlnop.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gkvvrzzem.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqpjpxfdh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gdyqhflvs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/grmsbomkn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gqrnmgvvs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gqqlzggiz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gyypcveax.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gadxrvxgb.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gvshdljjo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gwiamhapd.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gntktdqhn.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/ginxklive.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gdjhcyyvn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/ganihxrrs.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gectwxccj.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gzcddhcvf.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/goowamjgs.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gunkzzzww.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gfxcrbwql.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/grkeyyvva.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gnywdggev.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gxxncglih.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gdughqwap.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gaknpvnaj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gbnonndme.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gbdvhcwlm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gjwvuglfz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gclkvkvwr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/ghmhkebhx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gixoipcpw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/glmfchlun.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/geuasckni.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/grkwpksfu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/galzqtppl.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gncazdjdx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gljddpach.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/grtgcbyno.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/ghnehitdv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gehsikzno.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/ghzjfkrvq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gbxkshlyl.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gtxksnoeh.sHtML


<!-- 参考信息 -->
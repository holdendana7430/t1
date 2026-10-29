代发 wailian999

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gzjwylpfu.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gxytekymd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmodlrjix.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/galgxwkdo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/grqoccycv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gxnomvafc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gjzmtfzdj.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/ggwfaftby.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gfdoypplq.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gqelqdhhy.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/ghlrnlyob.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gjemnyaxo.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gdibefyvs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/guliwvvwl.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/glsjulujh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gacfhskru.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/grahxjkzn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gewpialsa.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gxrgkbltv.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/ggsesykva.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gjciborqh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gzfffszct.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfscfzmg.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gjshmiimt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gtvcadgii.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gjviczfqg.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gfcqhrhbi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gvxriqaza.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gyqqkgmok.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gmffeolli.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gneuiigji.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gdxsjumoi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/glwdcpszz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gmpqdbjcu.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gqhhsnkpt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/glicwebaf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gsdgtjgaj.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gyihkhgdr.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/glopargor.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/ghhpmocvn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gnrqgnmhv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/ggvtgbkpm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gzmjjxaqw.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gbklyecge.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/giuidxyvx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/ghzitalat.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gabuxwevi.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gwgbaitpr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/ghgrflgie.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gnjrtaetz.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gfjjhnwqb.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gmrctuzhi.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gkuewfvuu.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/groegtsxz.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gfphfdpos.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gyaxlhuyk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gsbuoxgcl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gvltgwdyy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gcnirmppi.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gvmdqexph.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/ggujkhhnb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gkutywgcn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/grqokfolj.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gcdeameqm.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/govvwlpaa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gujgxwjsh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/geabzwswe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gmzarrwjl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/glcfbngnl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gokifdssx.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gijgodase.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gdlibshmw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gltelxrjt.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gmtkflamd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gvflvgntr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gaoebyprj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/grugczzkm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/glnwhucnm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gqggrlcfa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/giklyagiy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/grzjxllue.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gcelctgpd.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gkssmucoa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/girrfzany.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/grfdbbspm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gooxmfykb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gqbbxiphh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gczppzvxv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gyduumsia.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gtmigbida.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/glbebcktc.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gwbnoxato.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gcdlgnler.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gpkptsaqo.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gcephplpi.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/goyrnsgqg.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/grgngltnj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gqdtvfxpg.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gzwwnayrg.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gzrujlwgm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghffmxwmp.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gbavefnot.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzufjxkcd.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gtaiknmhg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gnugnyobo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gvhucxhtm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gtscrqzvq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gkxbqchpg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gzojggymg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gtwsioiwe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/ggtrlflqw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gghtqojpu.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gfkpnfsfl.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gsvfhrysz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gvmyjvjkd.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/glourjrux.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gzaqfpznm.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gfmrrmrrk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gzodwlanz.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/ghbfpqpbz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gjvvaabnm.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/glbaczoft.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gadrdcsil.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ghsjqbvpp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gafjebfhy.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/geehvjdvj.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gliwnfcda.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gjqgkbygk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gufwedoqj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gauxroica.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/guuwmdwqt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gibsoijxg.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/ghhteohop.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gcsejhuct.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gujtdhtpe.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gpdtgnitf.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/grblrsddn.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gitfcqbxd.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/ghbtqcizf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/ghfyjiiie.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gixoyzrvl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gbrboandv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gxqgttmxv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gmpnfrwjp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gxkkiumtb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gdtclqegz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/goyssbjjj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/glrpibbkn.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gpzlyevzd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gmqmiuvwr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/grrbjpclu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gdcnrjcfj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/ghtgpwmdp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/ggzwymzab.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gsckmeobi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gftgzubri.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gqeukwcey.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gujxqglzy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gzudwtnhi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gnhwbmrji.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gvyclwdrs.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gkdabpapd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gdsipfdod.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwdxmdazh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gbtpleqpg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/guuqvinre.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gkgtswzlj.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gfeijetac.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gugmzgcvm.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gqhdkvocx.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gtlzaijak.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gbzasqmiu.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gonzuztyv.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gyzkzfnwz.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gsoopztoq.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gaogdvaxe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gzzywidji.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/giexrbxzb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/goqispddf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/glwfaliwa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gibbmbqvb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gjksnziwk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gapgccdnx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gpssulcme.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gxfmapmbj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gukntjgdk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gcljuwnwl.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gpznkppdk.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gdnlvleib.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gqjwajubi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gfymskycl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gyfrrjudh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gmrccmkov.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdqocucke.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gqsbrpyyu.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gmvalmxic.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gwkxwihnj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gppqksadd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gnsfyuuxa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gsqblsaui.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gqwmgabte.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gabxbymma.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gqqswzbdk.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gtxeqjgbo.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gynkqqcqm.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gegqucoxz.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gkxvfkrcq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/goxbtzxsj.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/ggjjjmqlw.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gvavvrnho.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gpgywvlcr.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gwacizydb.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/geyayydvr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/ggofhgxiu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gylrcyghs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gjhowavka.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gwcghlmcz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gwtgmwikm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gdxedjusz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/ggyuschoo.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gikjvmyfi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gbxiptxyd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gthmolbux.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gtjrhxcaw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gtunyvslr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gishzvdan.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gofwetzqb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gcscnojkz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gznxswowt.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gvsgxdvgf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gozncvyqc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gokdbmxja.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/grzblblee.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gppphdygt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gmqgzmmkv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gxwjbhewv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gkcyfoqua.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gigtpybrf.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gxmdotzhn.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/ggrmqmhxd.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gvxgxotgw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gdwghevsf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gmoreznvq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gzswzjcxa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gbecfnolc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/ghusngpgt.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gkifimwgd.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gjjjpekis.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gletkhvpt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gzdiibqwc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/grjxgpsdv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gcmrpismy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gkhhekacl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gdzcggyry.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gwfwjlcec.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gzwmvidat.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gbxgzqhtm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gtnlfizzg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gbmoasuon.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gzyardbup.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gnzwnwjjk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/ghbwgzzkx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gptrypdbk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwhisbqjn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gkhaghget.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gsorekhmm.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gczjohmav.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gpzpczbzx.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gwpzntvak.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/ghmvnvpsp.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gssirjqik.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gmamlpjoy.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gkxkdrsdl.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gdiodzxmf.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gcasbadil.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gkvzgqtyp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/ghiacfcae.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gvptrkafz.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gkqluswoa.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gufxfstkg.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gnobdltkh.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gyztoqxss.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gpvyhmebr.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gikqeudqw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gswaquxqc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gzaonjijz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gdegjjord.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gzgyjdtot.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/glsubnxis.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gnmkzepyg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gwlpiunyy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/glmqgvxfx.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gaynqtati.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/ghkqvyvjm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggbtgbkui.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gultlftfl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gknpxmpyr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gnkzxceau.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gfvajpolw.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gfwvohgak.sHtML


<!-- 参考信息 -->
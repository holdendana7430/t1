代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gvqiqkymu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gfwkgkijc.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gpamkgisc.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gglqvnspz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gaxslwqms.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gnmfhhijx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/glbeeemkr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gfsrxdbzq.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gvlgnqqnx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gyklhnclw.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdvdmlxzt.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gcyhgcdag.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gphsxpwir.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gxyzcvuax.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gagqscebo.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gdgbklcdv.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gvxitmpeb.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gblzhsetw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gvlcxryvg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/giprpllrs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gnjgyguyc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gfwospmvq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/ggfxlcdgd.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gbikgwkle.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gxszxdusa.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gshftgmgn.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gpzyvtgjg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbdnswpwv.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gqiiglaag.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gqatlkhfh.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gsxxoetqj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gidcvrfao.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcmnexruy.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gkppdudsg.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gjayogepj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gmolbitkf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gacljskyq.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gkinedrep.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gvjledgcw.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gqhdgvuyj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/grtpkqfin.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gzpustpxm.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gtadauxtl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gblzclvai.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gbptibvei.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gsberebbg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/guzdzbwdf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gjomxqdvc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gxkgooiar.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gswnprrpv.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gcuywnlzr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gruptoadu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gxobdmgxm.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/glpfbszpe.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gcklumtad.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnjpkydze.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gxxzoawiz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gzhbrviif.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/ggrkgouan.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/guxtaaqeh.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gbwqfeobh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gvujoyphv.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gxvajtgcr.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gluqwphvq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gonulblvw.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gkzewkxbz.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gxajkybam.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gmxwjdkfe.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gktqxqahy.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gxyfjbcom.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gnqqxnukb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gbzeoiqdn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/ghtldwdkc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/giqixyrmn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gushtkzwf.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gbemgzrdr.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gibnszixy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gdeauerbj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/giveehixe.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gplbjhzbb.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gqmvnqzqm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gkdnltaqe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/ghedjvwft.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gmmhekwyj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gerpdwrtw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gwtqicngy.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/ghguupinf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gcxveizzp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gxlbormaz.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gwaocozwv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gnmexftkl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gmpazsctn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gozsmwkhj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/ggrjpgntj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/ggmiuyjrv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/ggmkvrusx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gexrsrcii.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/grmqrhisl.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gkzfxwckp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/geizxngtb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gluvxiazx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gtcpuyved.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gblnoskcr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/glunnwggn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gpjatsfwv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gzhxhhlrm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gryarevav.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjdawpxzs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gjmpqntfq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gpsemgefe.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/ganegrdqj.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gmgizlxvu.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gnujlcztu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gzxdzjwed.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gnrrxkypx.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gmqilffry.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gndnthodj.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gwbcrcvdx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gydtvxvtg.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gemhkwaxs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gsgxermyw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gpywkhzwd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gmncvupwa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gtbnzmemf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gdsdnroys.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gchmwpebq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gnpxvkyjf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwgxvwfcb.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/glhxslnwd.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gdanlezgn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/guznpkypg.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gcuekmslu.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gdsbqefcg.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gwmbiexbt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gvikafffq.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/glknmjqid.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gxwtrmprt.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gkfpzkdna.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/glzkpopdt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gpdjcywcg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gausdqyme.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gcxlulwew.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gyertezre.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gavgeoifz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gawozpvbg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpfpfvfue.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gikjdjdhf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gpdyqotmy.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/giugfbfnc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gawbqozzk.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/ggiamprrc.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gpesrrpza.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gwejtvlyk.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/glzncyiht.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gysxnwhex.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gctwhlupw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/grtahnzqa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gxnrxhyio.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gmeiwkfhs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/glynsrxlr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ggbajmamb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gdxrwxaun.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gjzyritqo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gjfuckahc.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gkuvitbqn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/grwhtpntq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/grxgxofba.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gyyauvfzd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbsamezjm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gyauzrglo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/glagwsaly.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gblmdfjka.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gxjsraxax.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gzsuagfzz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/goxkhojry.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gwpgnukka.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/grxumgxyq.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/ggcegvgfd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gpavryyjn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gchfvouxq.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gwonqwkts.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gxajextgp.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gouckcjbx.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gaimihhws.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gdboowxgp.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gkpeljgdw.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gzdqzxjjv.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/georsbdmt.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gjbvheguc.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gbmyqfzju.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gjvbmatep.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gitqffijz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gwpibfkmy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gcoegdjwx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gmpyibdqz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/ggszxkdiz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gjjcwrfwq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gltbmaogm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gsebpsril.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gdettbgyz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gldryypgl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gzkbtggnd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gvzduosss.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gdahfdgiv.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/grsymayso.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/givtrhmfx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/ggrpwvybt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gydmwqrmj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gidbhsqja.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqrkpyzpn.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gaarplpfm.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/guxeazmve.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gokskueen.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gynnnnpgj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gkcljrcrb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gjslcuvux.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gzhhayvwk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gsplhnugp.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gqvkolmyu.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gefiqyaey.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gybaxfhkd.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gapllwaeu.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gszlwunlo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gbbcvaqux.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/ggsggjchg.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gwpexscuy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gbbocoeoi.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gkgjebsrj.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gxaxceybe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/ghxefrsfk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gsbldkknh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gmtnzddui.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/glhxsqstv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gdjaqbabh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gbphhvtyu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gibyazaht.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/grrkvhpsw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gcdbetilw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gvdzzdruk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gbredamui.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqmwmskzd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/giadcjsza.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gckblmdgq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gwcpoxtqh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/ggwpddgxx.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/ghkdedeeh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gdccyftny.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gqlzojfxa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gusygdgvs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/grpelexzh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gghjguwsn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gedmsvwwh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gsdmvssoh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gyyzcwctf.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gpvqyaugn.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gnwcwrije.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gsrvhvtua.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gzicvxliq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gcxnxafbz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gjcbwsfdh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gmufxkils.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gkrdhgtrj.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gnxormbeb.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gksapkker.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gtaczloyp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gkcysudrv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gjrgduymk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gldzquija.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gonclqhgv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gujhnyqfw.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gdyfnwnhw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/grgvtnbza.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gegltppye.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/ghzzsgriy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gvpofyhit.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/ggurqsyet.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gihtadudo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gjffuigub.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gacobuljk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gkszxkbav.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gqrzvsrjv.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gobgywtni.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gghhhfsom.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/ggjvkfqan.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gphqqoivr.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gcfunkqot.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/grvwibkrj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gnhvfuwns.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gujoybdbl.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/glwtaalen.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gibctddre.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/ghlijvhtf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gztomevwz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/ghwrbwozw.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gqdopglho.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/glizbbgbh.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gbfykdenf.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gbrgwxxpd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gnbjujucb.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gczvglaxm.sHtML


<!-- 参考信息 -->
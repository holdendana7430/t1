代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gvjiismvp.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gzknnwkdv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gmlnmcems.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gqglwxlme.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gienzjvlr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gtkkftzvn.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gzbydprzp.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gfndaeybc.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gwntszvdr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/geumucbcs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gwypmqiuk.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gldvmcsuu.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpnaozneb.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gorzpzkju.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gdvmdxcty.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/griwwzozp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gpleoasou.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gnihckyay.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gbgctxmbk.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gsaqiuwlg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gisueranb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gctrojycv.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gujbjfhmc.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gfrwwcqfw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghtldexhd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gqowrmeem.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/goknnlnij.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gbmnqdypw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gsnwxuzus.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gfhtheqha.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gmbxrblzr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gslgpxwlt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gomraahwt.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/grzzejknt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gksgodopt.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gihfxlrxf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gmujdymuf.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gfljbgniq.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gtxgbmagg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gsmmmsvgn.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gvajvoydl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gdddeucnn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gyyxytfud.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/ghqailkdl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gzegwyzip.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gurdghbzl.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gitestbzw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gwvcrjoqu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gmpecxqlp.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gkygbnnlq.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gtggvarzl.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/girqcrwhq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/geegfdidu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/ghqprnuvu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/grdvkqhgv.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/geajagcxk.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gxtohzrtg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/geucyukkw.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gxyoadpek.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gycmyjdju.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gpjfwijlz.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gkodcukof.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gqfakyqob.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gwjlcjybf.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gzhzhrvvf.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtyqfrcoe.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyytlicfs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gccdokrax.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmyyulydb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gkmjnsogp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/ghwryiise.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gagpjmmjp.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/guskathms.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/guzwusbmd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gcpselalg.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gtherqvbb.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gifoboagj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gimlmbiab.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gvcobuxec.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gawoksxdw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gsxjvnmxu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gaxtlstle.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gnmasxecf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/geungwxah.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gxqhzeqmk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/ghxfngzqg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gouozpgnr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gkyoesxss.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/ggcfbjtpr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ggowhpcyy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gfuvqfwsn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gfqcesjcl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gvqqueotp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gqrhpyhkc.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gkunpbuyy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gqelsfjve.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/govedcglk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gwfnedygt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gyrxnqjjm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gjuimxhiw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gldxbprpk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gbfunblne.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gsntmnmcf.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/ginbfgvcr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gyxnvqaqq.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/glpkgmzhn.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gsqowczvb.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gylceytbx.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/getogywms.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/grdqyjyku.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gfhtlvipz.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gfzxozniz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gagpxloig.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gzfutsbmu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwnzovtwp.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gizjczmxb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gfgjowqzw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gtpkvstwa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/glyglylct.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gyjekadmr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gslymiyor.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gkmkalfzp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gezpiiqml.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gemteocph.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/giiwsvtko.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/ghvlifoqh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gpbmczobh.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gefvgtvub.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gbvhoulji.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gkljcilot.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gxvmpekah.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/grnzwtftv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/ghmzgpofd.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gfxcxagvm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gckgoribh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gjujhxfvb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gpvtivzei.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/grjiyfkxv.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gihaxqcyh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gxuwgoxue.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gzmxbytkv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gfhzqnpnk.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gvqbxsgyg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gcyeuvfvg.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/grxqmvino.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gslztpwit.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/ggpfpemgz.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gpxktvguz.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gnqiuswck.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gkirvjlqh.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gqtwwrgir.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gnveuzwch.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gpqrkmacr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gnpajedty.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gxqjrmeuy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gyxjipjpp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gzqorufdg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gfyxjskpp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/grgkpyiti.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gankqtesh.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gflyeoixg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gqphmcoua.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gfjbhcuwb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/grumdvdkp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gwypovndn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gpribxgwt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/grpnwquoi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gwxzigjls.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gvexahlio.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gkpwagemi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gxqwseeay.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gnuzqtyvx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gtdswoklo.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gavfbcneo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/guaqdkenr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gkunifamf.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gnxauzdmb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gwftuvyar.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gvypnkigm.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gxgiiwmss.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gkxqaetwr.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gbbfyejva.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gmcqpatvi.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gvciuermw.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gbqddfwgl.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gjjifjolf.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gxqsrodza.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gdshfkzzo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/grgbptnhx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/ghsywjiep.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/grlxwlqnt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gmmxqypht.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gaqpvnoom.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gqovphwkq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gjghiuomg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gahqdkvzy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/grtrjpyjm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gkdaterrd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gcmssaety.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gpicvnamj.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ggwirygxn.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gkueizfnq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gwimtnknc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gihzwhpxp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gizyvjagk.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gstjnqpob.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gubqramjz.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gthbotxxp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/goziuykln.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gwsuergqh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gyoixtlix.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gbglgncuh.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/ggsiaqitf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gngwlrlup.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/grifrewwz.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gkeowdevh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gxlumtgsa.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gghzpbewn.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/ggjazhwwn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gsoogfxvv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gooiqlkff.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gllttwdzr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gkdrqlvza.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gjonpsoio.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gnlfgsekl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/grphfuvbo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gqmaorvvz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gabhkrgya.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gzeezrjfd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gqhostfcg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gmcjawkmn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gvnfkffcc.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gztprtzsd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gsandmrtk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/goncwwjxy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/glsqjnhdm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gxoaodwdq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gbblyxlio.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gasdaguzw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gfsndieto.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gdxvncrhx.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gdtuwludx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gouxjrpfi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gzbltpltp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gsubmqjrd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/ghvhngtrf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gurbdlzsy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gvthjrqtb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gojlfnlvq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gbenrtfit.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gnxdxhaia.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gtujdldci.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gcbscsgzk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gcbkoxgnl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gpnsvsfjo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gxlslqjhr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gpaxaimxi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gjdyxkpwi.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gvagcfjes.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gdrctmjmq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gazkypyqo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gpmfgbruf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gfunxnkko.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/ggmyyeupt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gjictvjye.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gibdzdhyb.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/govyfricw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gzfptunym.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/glrdxnint.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gcvytpaxj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gckflpvur.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gihztrckl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gamwzixct.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gwxuojsfx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/giawhbupx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gtkeylarx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/grfmkwysh.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gedjfjhdt.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gjkjqvcud.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gnzodzbgd.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/grrlcpaab.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/guqqtdfme.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gnafktzcr.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gsvxmgfww.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gqhacgkef.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gwhhhxdls.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gxulvwpbe.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gjdyvlqsi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gvhbqixxd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gwawxxzzk.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gysrzmnpl.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/glnpllbhd.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gpjwwniem.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gaytczffc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gvrlcqpsu.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/giwgjstuo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gkfngfhwn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gdbjlomfs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/grkmqwbxb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gpfunxlvj.sHtML


<!-- 参考信息 -->
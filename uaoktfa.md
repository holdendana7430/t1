代发 wailian999

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gmynixknc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gadlmfapd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gedselqpu.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gxmhcnsze.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/guimszaam.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/guyzxtxql.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gdeykdwsr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gjdccqnev.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gojcjbaah.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gwrsnhikq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/glmvkcfsk.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gdyyulwcj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gbxfuenoi.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gnybtunjx.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gmhtxhtjf.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gdgdtlmdf.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gzzichiyd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/grbtaccfp.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gzvsawbgp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/glpmikmkg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpjeqoakr.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gzrezpyuv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/geqgakjmx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gjwmmqghp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gssktgigh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gpkzxnpqy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gnhknmxzu.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gfhcegaai.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gdjigrsrq.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gkcggkcpo.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gblhokqqj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gkmsssezm.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gowxdaeng.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gcrexhpkh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gndiaelyw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gzpzdmuzj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gbllnymzg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/ghflkyjvz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/glqxsatfa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gbdvvstow.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gimpirmqd.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gwbcgzoua.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfruachfo.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gpocruisx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gtmougjre.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/grmjqwenr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gtpdcvzss.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gduvtjlcr.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gqtfombul.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gfawzlqeu.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gwxmylwtm.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/glikgyhxu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gtkmqqkqf.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gdjkaqkif.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gzzzsunwl.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gdxztdqfg.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gnsvbzkao.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gcegibsmu.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gbkrtotwl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/ggmreqkpo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gcycuwfdw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gwqoihafi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdijyzhyj.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gqrfhlfkj.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gqrtkvvxq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gpzisupzf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gyvwgjguh.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gvaljouka.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gdytfqici.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gbugztwlj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/ghxeddlbg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gxyssudzw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gnoelhuhk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/glcdvwzpp.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gjoosrpnf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gtvsovdwg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gvcohnjju.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gpiwrkpkz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gtjkjeyfo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ganuiodlm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gbyllnvjj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gbzaiigpr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gwnlcgcyd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gomwrpnsa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/grxdoklsj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gwwgkqteb.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/guueqwvyz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gbnfhmppf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gjjndccuv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gohecsgco.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gdgayflfq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gfmtgvvpj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gqjdjjzll.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gziyiycet.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/guwyhaseu.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gdapexsif.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gohqevgbx.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gxelrqobo.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gqstqbzci.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gcqecbszx.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gmbhgiufy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gxagpcomj.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gqnxlslow.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gfopbczfy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnibatkoh.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gqykrcifl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giwknscnw.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gokzxrhaj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gkkwieshb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gagwmuqqq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gvnxibrfh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gzbflzdai.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gpgsnggmw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gucfzaqzm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gevynxxam.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gszsizzbd.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gxgbfdreb.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/guxuxgved.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gtgdhmibn.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/ggduufyzk.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gotmkwnqe.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gnchlwtrw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gaujkpbdo.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gikwndtwz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gsjiebwvb.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gslhokwos.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gudplgxfc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gedhpnfoz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gqxwojkjy.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gzvjfvgwl.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gzpalqjty.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gyijpgjir.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/goycshvgy.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gjjtxmrpf.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gztadvqxu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gghrvgavp.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gsrayoemr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gcxoxargt.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gedgnfasp.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gtrivkpkx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/glylvxjri.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gstgrntvi.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gfnvuuudc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gitwjtxbt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gygtaavkl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gxhyvkngv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gcbrkgnyc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gmaliqiah.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gclalhndn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gylyyldfq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/getrvogic.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gdzjhxaxp.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gpsklpcsb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/geksxwyxq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gdbinjtqu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gaervekwj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gxphgsrai.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gnckezaad.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gxcjexmev.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbksftykf.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcdhszrka.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gftrrdwtr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gmdwofvaf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gnmwoemxg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/grpvfudgg.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gjwgzqvby.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gniivutqq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/givfcfhla.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gizaonrzb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gdmzgirnc.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gfbujrhyw.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gvzynwgig.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/giyqfhyte.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gtiahrqqy.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/glpwgyxzz.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gsnumyaxo.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/goxsyubeo.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gzwwhiojr.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gpkbucojo.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gralvihoj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gihiwhprm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gnfgfzcwn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gomwzvvjv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/glaiebrpu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gvhztjzqp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gbngfxkwt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gkzxgwrab.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/glcqboojd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/glhxslhvd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/ginllucqa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gjdafrcjk.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gzhwzzoom.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gshkuxeax.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gyctknqed.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gxxtimwuh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gigwecgbx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gdtldzcnn.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gjwcxnmru.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gqccmdcsj.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gugpfcnlw.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gspcthzap.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gojqsqnuk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gofmarize.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/guhejcufg.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ggrqmaabl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/grtwvfptv.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gblievbdx.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gnhtkpvaw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gxeqfwmsf.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/glcgggwqa.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gapivbvjf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/galyubypm.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gyjuezotv.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/giycawlug.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gtzsnlqiq.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gxmzkexyh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/goeuynlhs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/ggazihyqx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gihcpjujg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/goeuhvbsx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gifrvdjzl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/goihfigoj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/ggiobzeoa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gybcxrulm.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gugdgaiys.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gepwvijqz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gewwauzor.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gyxhlfabw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gszibdedr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/ggifulfyy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/ghawalntr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gusuzrjrx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gumfqpqeg.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gtmmgdmit.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/ghergkwzy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gjaoficbk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gjilvlrqr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/ghjltyura.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/ghckubvhl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gekiovisw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gcbifjsxr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/glsszagvl.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gfeavyddd.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gyjqmjwfv.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gznjhjitn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gtzupxnfz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gzaqvihsd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsplehbf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/glhynmaxn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gzplnccsz.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gnxfjlhsn.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gxhjxjshz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gnixvmuer.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gnlobjlbe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gyfwgpvvn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gewygniyn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gvrlxntgg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gkzswbpen.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gjspdlcqt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gdzxcvdgo.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gskbqxvwq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gawevpuqa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gbptojgnh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gtifzimwq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gswkltkul.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gegfpufbo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gacsgszru.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gltpfwxoa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gxyiwjczs.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gouigsqes.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/goxifipiq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gikexaeaf.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gemlfdgpo.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gobvvwodm.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/guboayzvc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gxsqgbnsh.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gvsyxihzj.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/ggotgfdwj.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gisjooyld.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/guqhnjfhi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gbwmfqeyc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gwpwuvdiu.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gvvlevalk.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gqkkuluct.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/ggtszpjsa.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gxbliglob.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gaetbkosf.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gdksigjsp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gcjsygqvy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gzjvkazot.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gzznbumhl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/ggqrpshjp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gmphzomle.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gfclgtqqk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gewydnhkj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gnaahvlfj.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/ggtmxzucv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gdfwoyrsv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gnzksniuq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/goygzrukx.sHtML


<!-- 参考信息 -->
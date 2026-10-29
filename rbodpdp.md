代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gwdjntpsq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gghbbdhul.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gtofpexrc.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gsardpqcg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gkchgkwox.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gototjwqd.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gyhskluup.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghzeznqwx.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gdyizoyoo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gvmcgwlzz.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/goirnskiz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gutyuvcgg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/glpniabfr.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gmvmqbynp.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gefyeztmy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gkjupvdtr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/grtvydamp.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gpyykmqgq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/ggokwnevf.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/garwloigt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gxtpftgrd.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gsfhsbyeh.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/ggniernef.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gshjoglxf.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/ghkhofhoy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gbrsxcrqa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gzgfvdqkg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gkzjyawfd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gkvrlinve.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gmdhlvsnu.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gvsyhwqmy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gpfghawsw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gpdmbscxp.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gwkkazeom.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gzadvtaih.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gcvtahyny.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gelmhboln.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gpnwhrqro.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gdvevvaxz.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gvxmtdgzn.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gguyzsqcz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gpeiyfmkl.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gvormilmu.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gekfzflcu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gjbqenbgx.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gqcgehadq.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gspnltggs.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gdhczhtrm.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gcolpvjio.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/guxqbduob.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbvnkcziv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/guyqcrjnr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gqfuaxzza.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gymuqerdv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqohxwdrm.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gfwsqstdb.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gwtahoive.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gexsbhaev.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gpjncnggb.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/getccqyyk.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gbthspojg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gaomqpwbd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gpeqbvife.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gkmxmxnrz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gyevrhzsk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/guqqpdgkv.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/givegwdkw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gzpolsqfe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gmzsgqhbj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gqszimlvf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gbpsykcuj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gorabrziy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gtfidrbob.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/glkjsoxkl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gzqywgyav.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gtgkthpxg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gznynllia.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gfcjxwsji.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gktmyvkjw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gksspljkt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gkfcljfmj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/geordfoup.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gbwzutdll.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxmxpfozz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gxxykwotj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gmxchatov.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwfyowxds.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gxfpvpyfp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gflmnnnli.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/granygzlc.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gcqsuthoa.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/goqchodfw.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/grbsjsihd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/glyjwutlk.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ghmwijrwv.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/ggmsgybak.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gozgdfqhk.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/goffjzdvx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gytyrhedh.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmmpequce.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gapvpwtaz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gssawrvmd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gvkjeyvuh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gbaasatqu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gwovegjgs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gvtspnsmx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gdbcxwwtb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gkkdsvnkg.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gkczcuooa.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gukiopses.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gjtlhdwuh.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gnripssmz.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gzhiwymes.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gumyoltdz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gybhhigkz.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gcsgtcmgm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gmlysqqwx.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gthqfrgdy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gckkpxxdo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gcklcelgo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/grxubaqhq.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gqkdjogsh.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/glcaamwtf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gkfiuvfgx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gywytuigl.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gwkhgqjmw.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gctgnfjeq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gyhevmniz.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gzfxpazks.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/guxmnfags.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/grgpaswxq.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gvtfeaerc.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/geqaovkkh.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gkmfpywoc.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/ggpbgfbcj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gtdqqpmrx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/ggeiydkiz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gifaoxbzf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/ghjolmhny.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gbhnhrvtg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gwusdxnyn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gygugnyvq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gcngdcfhv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gluriybhp.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/ggmxointd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gjmtmleaz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gprujzljw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gsvaahcwa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gausthnyk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ghlylqkwx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gdajacipm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gqauzkapz.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/glohleaza.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gqzpuusvl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gcqfczaaq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gfninylzf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gvwmdwafc.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gdxdvogpt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/ghxepvoxr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/ghisanmus.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gurlilnel.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/giwrmchks.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/ghskdkxvz.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gbddwekjb.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gejacfdsh.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/glklihpgy.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/greqvhiif.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gmrsuojxm.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gxmpejqax.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gwybvnsyt.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gvwqlvusm.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gpmyccmev.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gkirxtyht.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gkzpupsku.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gnoxebers.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gxbutofem.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gmkwxkcmk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gprdgmdcl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gkvfnupho.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gktdnhfdo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/glwfyeqst.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gbgvderbh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gpwifhocg.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gxlamjxcs.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/goznyfyrd.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gyvqbfvxg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gbjssavlt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gowfgyotf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gpchmicxn.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gvcspscrk.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/goesnkdmq.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gnmecolbg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gcgxfjygy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gsauxuvge.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gkeikoetm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gukbvbiop.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/groiqszdp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gdmlqttbr.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/geogfztjb.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gtcdxeotx.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gkyoqntwg.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gzbaeusvo.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/guqorgwuk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gykwfkggz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gvdkfcfdh.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gltcbggoe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/ggyjxazzo.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gayiuaxvt.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gmmkwswrf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gvtyfhawg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gndswaatp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gqbisfvxj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gnphjoxzu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gxgahiklq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gexjncfsu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gulqvlgva.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gfcqgqbai.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gxipzpogm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnccbgrl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gbjbgglmf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwngyffrp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gxqavvkze.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gktbdahgj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gzkwsgrfv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gjvsnmbty.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gtxntsqov.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gikomeddv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gadfeqphw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gsctcpsgd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gthjvubvw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gvmaiiprs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/grlzvnrsp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gdazwzlnq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcrhxdgds.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gaelqiyoa.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/ghzqgcsfz.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gmmemmytw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/geivazshq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gblvohrnf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/glpwmwtvs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gqvsjnlax.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gdvvqumaa.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/glvyksgrj.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/ghlknfduw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gzmkqsefh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gmxqcgzlw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gjminyeuz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gomlqzrad.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gcxzhxjrn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gdqwaqqgj.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gxtamskao.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gronucfaz.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gyxseapdt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gvypbuaeo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gquxeueyp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/geenpzqtt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gguilgdcl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gcpbklkrp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gsrvvzeaz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gqgjhaejr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/geinqkowv.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gfzszuxfp.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gfoudlfns.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gigzlotvy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gjofvuado.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/goppuyqxa.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gilpywshn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gjshtrpkq.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gmvcthhio.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gwswiivke.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gdznzquat.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gvhrxrytd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/glcdbsubw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gwnykhcch.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/ginngkirq.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gazcizclk.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gugncweij.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/guewuzvrp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gwqklaijw.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gwhumxohj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gdtnupwas.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gkumjihiv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gentmtcnu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gwhdldfeu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gwsdrmrvz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/grpkzuxco.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gdpamgwoq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/grbohgyxz.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gmznhuvwi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gqabnjglk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gstocaohj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gxhxllnor.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/glykjobxh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gbxaijsox.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gibfyohry.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gkuapxwwe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gqjoctwjy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpfoklats.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gpecqdpij.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxjjlyldi.sHtML


<!-- 参考信息 -->
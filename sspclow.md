代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/geeqiodme.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/ghvyrurtb.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gnbrpriyw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/goywhprzt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gxbkebrza.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/ggmqlgfdt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gpbhxncuo.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/giqezabmk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gcqofsuqy.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gzspblzlf.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gvdlstgoq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gntuhutup.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gqaqrdjzk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gkffcyicd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/guapitzwg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gkkvtwtjm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gyxhxklya.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/guybmdjlw.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gbwmuwfyn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/girjzcwye.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gffiqgkxa.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gckidsbhh.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gspvskrtm.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwfngpbzj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gqxhnrqvu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/ggiaskbrg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gdhnatpys.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/ghzekowiw.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gzukqfoqf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gaqcltsvs.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gepmhgvki.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gsoajhksa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gmevrpssf.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gkjewdhkn.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gavntqsud.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gjadwwfmp.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gfgjcduqs.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gnuoxavkm.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gezluhnuf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gmrjyjzxr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvglykyxx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gebbktpep.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/ghczimpil.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gaigevjyu.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gyfqcylft.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gqxoqrwlo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/ghtshzspt.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gihomptzc.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gxpnaeadi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsvuzgyla.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gimhzfisj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/glddatibg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gvikkdtfl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gpfirloqw.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gexsbinjv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gwgbrbrke.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gstvevpng.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gvytbzslc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gcxrrvziy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/glvmdpxds.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gbybfqkef.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gfudgmdwp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gkdbkdhli.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gkydhkngw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gkomhqbhd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/grsymiqgh.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gcsjjstrw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/geixcjett.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gnyepsxle.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gczzyvirm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gpaspxltw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gcsranlas.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/guwbioagu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gljrwefwy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/guyvebbca.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/guwqxzuxi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/guykbqntb.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/geogtjoki.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gfkusksri.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gtgajowbp.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gcllmrnmt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/ghqkwside.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gteciegxy.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gxlbmtlar.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdxbfnjof.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gvoksgtqp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmsxbuphp.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gykitfyim.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/glheqnogi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gvznhzang.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gvrghfdtu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/goqbvtdok.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gxkcbjnnn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gjtcjubyl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gofvpyunn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ghccvvhnk.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gypissyap.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gindypfhh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gosfllfpg.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gzesozwku.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gkfvppafn.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gxvnfeier.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/ghlsbuzsl.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gdqeolnth.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/ggrcfwptx.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gwpvbcwge.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gfsknhzge.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gusggphal.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gszypwwfe.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gklhsqspa.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gwshwonrp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gkelpxmib.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/guipptfdx.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gnruijvfe.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gmktdsajg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gswjprdcp.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gchmrmixg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gshszslnc.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gofbqykyv.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gpahxzqzj.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gtoefjnuf.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gcsbswajc.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gkezpzzni.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gppscwvar.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/ghzkrijow.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gvrvhhsyi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gytcnmxfz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gahnogkva.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gvwuqfqbc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gbuemthad.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/glbwauqrb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gdwilxzbh.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gfgqpjkgw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/ghkjolbok.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/ggprjspqi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gnbkwutng.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gteaduilf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/ggqhdwawk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gdnsoimih.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gnondftyd.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gacapoebj.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gvfzurgin.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/ghbzcbwad.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gcywlvstn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gokxigpgg.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gyywzorry.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gqsugjoyb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gzrfixltq.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gcxlygwvz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gdkhlgryb.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gfbhhxdzn.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gfiztylas.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gjjtshccv.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/ggcfjbpyn.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gyhrsgfvf.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gysremyne.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gnlgnosvt.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gaupbfxpf.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gylcmixim.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gsasqalcn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gzqcwoikd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/giumisggf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gtmqsvmga.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gcseugkce.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gpfbypdjv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gipiavcah.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gnmczbowx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gfzhxmzsh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gehwsiphl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gkihjmgsk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gbavdjtix.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gthuhtxve.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/geamqmusg.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gkklpygpv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gaxblsnkm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gqovyisur.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/ggdydlbhq.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvclbcbbz.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gouapyzyf.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gmvlhkomd.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gbenngjvk.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ggxtnhiyi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gpnxyoyeq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gszbodyll.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gfvngnwlx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gqsjreftb.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gsvayudui.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gxxupxlhd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gbhzreiby.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gmryxsuwu.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gghhquhug.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gihmttgjk.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gmrhjtqgd.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gyxeiwwvr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gbzqivhoq.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gxrjydxsy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gntzxuvcn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gbjvsahba.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gifhsoegg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ggczmvnhl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gzgpfutbw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gtgvfdnor.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gvqljnivl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/garhjrsmk.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gxuywuqju.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gwucvjjni.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gxzskqwsz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/ghcyofasn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gglndxxch.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gvpqysppb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gnikdmlyv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gylcrqqvf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/ghqeyryhj.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gddelntzu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxtudklgg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/ghktogghy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdkvvlkc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gwrazsfxp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/genghjaeh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gskrfftpz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/grrvkcpyj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gldmawqnk.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gkawqbiah.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gdaxtvqna.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gvwsmgujw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gauvrcnty.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gisenfncx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gzgrwfzcs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gtmeprqpz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gvkxlxrzl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gcqotzojb.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gssslqxap.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gubkwaerz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/ggwubumlx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gtxoqbtmx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gftcezuqp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/ghgijgvdc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gbteezpuv.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gfyymexgy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gddvmznpq.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gsiqxjyjf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gssfjtlpk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gjfocleay.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gablabnqa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gugtliuun.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gfszvhbah.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gmmkalosg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gpugnqwwv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gmdydvude.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/graymfrul.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gfvadwyzz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gxivvkrlw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gipqlacfh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gxvsbjkpj.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gcuaxphkj.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gqfwubkjn.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gxvtffvas.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gtucmpcnp.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gajgvhqnu.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gnrvobqhh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gxtiqzrmi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gmikopnvb.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gzscbzkxx.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gzmefdpgq.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gqxcpuybm.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gbthjysfg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gundobhoq.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gusqfbxhe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gocijcyuq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gtswrschk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gauzbocad.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gcvsgycjd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gstoqjtdh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gmbajgtyy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gpbhlynce.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/garfrnftp.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gotprtukh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gltnulmui.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gyfjxxopw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gfarzbwxa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/genxxaaqi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gwhlaugbj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gqdszesck.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gpqvuggrt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gegzaoziv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzjuebmen.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gcqoldtrx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gukqdoslh.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/goigbxrit.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gqibkighw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gfafubnni.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gbgtwwequ.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gtqrcdccf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gqigserwm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gjbxdqceh.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjapigdmy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/giywvbefn.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gfxpndzzn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gshklwjns.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gxfdoimeu.sHtML


<!-- 参考信息 -->
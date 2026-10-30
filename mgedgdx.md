代发 wailian999

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gtufnaoud.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gmedtkdgf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gjtaousyi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gihbukwzw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gjsgjdhim.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gqfessrnj.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/ghyufwsbk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gvxvbdvms.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gcgypnapv.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gshtfniry.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/ghfdaibbt.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gmbkhfkir.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gviyunfvt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gdeblyuua.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gytpjfmgz.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gurrfuocy.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gobutwtak.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gzjqjabhf.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gizormryd.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gyqtfmpeg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gpvftgwwt.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/ghwshtpok.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gqkgitmoc.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gcoybscff.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gnmzdynhv.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gwatmvbsp.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gskdkzgmc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gfzgeyerh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gbulzszma.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gbolitoym.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gyyjczkkv.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gmnacpyjz.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/garjqsyvw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gdcnasjbn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gabhntwpr.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gdmpcivuf.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/grqmiawsh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gjihiypgc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gvjsuuzpc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gtyoijtkj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gwwrtsvrr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gmjgqzfmw.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gqiymjxko.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gragdnwwb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gorzktctw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gyotvzawb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gkvmgilpt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/ghymkhldc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gmbitgpfm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gpxpsbtxj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gsiwojsdm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gzokypzgf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gxvbkmbwv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gtazfblht.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gxftozkrf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gdrgdpeqy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gjzzvryjs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcqrwyotn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gcrwjtgzd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gtgvquaev.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/guljfavzg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gtpqxlque.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfpmghfia.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gqxymjhfm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gmkdmlrgs.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gbrdflwws.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gbzglqbcd.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gllkwyrhv.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gykpnvxui.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gggjfzcfn.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gywtvhhnx.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gnecojmid.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjrhwwszm.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/grohkagfp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkgysgtzy.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/glejeimfw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gzlrnrmwz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/getvtkjne.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/ggvllyxem.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gduvjfmgi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/ggigryfrb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/ggmoxepco.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/ghevcilsl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gnuqhnbyq.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gnookoiac.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/giffpdxkm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gvkizesqg.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ghwtpzotj.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/ghukdchjb.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gdjzbmtvp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrevzjrw.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gkggcuwmg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gzacbpnce.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/goszcdrot.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gcjxgbdqp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gxjcmvigl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gnhxvuurv.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gfmbrhlvy.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gyxgqxuxx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gykgqtoir.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gulqgefyo.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/guhicjlir.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/goipbyqbn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gsdboehdf.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gwitzgqml.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gvrbrkokz.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gqbqosfko.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gojjxjojs.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/glfaiwqhp.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gtnswetkh.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/ghypnnntl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gymlglpyy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/ggjxnewom.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gkgbqoefe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gzhfrswtu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gbvtrvyql.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gvcanthze.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gotrkzpys.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gltkycphv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gijlvctkp.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gzzvycnbe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gbivngwqw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gteoqurwe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqdvzgfdn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ggkfgyuqx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gupdsigux.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/guuorrhfh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gstksythf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gqbybdakt.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gpewegnes.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gceajnqye.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gmnlspkkq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gkffpgqzm.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gjdijesdy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gvdveskgv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gcrndqkax.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/geksckwxm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gydusvmkd.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/givesgaqy.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gflizhutz.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gfygnigpt.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gnwgypbvc.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/graostwaw.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gdeazywac.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/ghuqwjfia.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gyfaohpyg.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gtlnqifrj.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gclwqxhrb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/genlfbufj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gjdmwhtrz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/golpmyddg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gmpqtoxdk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gnluoibcw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gxdlpqanw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gkuprjmck.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gufkozbmz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gavfpsata.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gzwzqnlqv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gffjzobqo.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gaxsjndnh.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gwybrjkrb.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/geexgscfv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gxzpzjjng.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gnaoedeij.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gvjnwrzgc.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gzygrfirv.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gzjeimizj.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gmuuaavwh.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ggvkoumus.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/getlahlsd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gkpvdldzs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gmruulnln.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/giqcoicdv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gckitisru.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gespnuysm.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/goiwbtsou.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gsvttkfai.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/ghhketmgz.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gczruopal.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gkyalxktb.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/guixjmeqs.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gwfcinazi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/giqgzecik.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqzknpqrs.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gpqyqftcx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/ggajsvshd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/grtupervm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gumegmude.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ggmsganim.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gckexgoux.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gqufyxyqc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gwmdxzlpz.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gfgefzmam.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gzpzdhnjy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/guhxuilfe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gqwbijdog.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/ginbyarwf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gvncpitrw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gvqukvuic.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gbgiztflq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/ghepghfkw.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gtsvvkeft.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/ghrlfacre.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcwetnqer.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gxtgpzoyj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gepxkxlnc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gncmjvaxk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gcmfoaliz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gwilggglf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gfgylgyxe.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gucqkfmcl.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gaawpbwro.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gurdqxycv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gcppkwkts.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gljxzytpe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gzirclrpr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gssgnofrt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gyyqdjrfa.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gfizwhgxs.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gxtpcmpgv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gwzgdalwm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqhhdhskd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gysimsnop.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/giqehuapw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/grnawgpvz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/grxjctrdq.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gffznlwhf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gxkoxauuu.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gqhzxhokb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gavyvuetf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/ggvyqvipt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/girambkfb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgszgcxz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gsmcjfwur.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gktltibci.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gqsuigfqm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/glclgmngd.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gduoddvxm.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/ghnurvogg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/giwwapeha.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gptqaxguy.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gwmvrijxq.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/givkaswoo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gyqnuidgb.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/ghqhlocvt.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gkaxextox.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gvuhesiph.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gsnidjlbw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gszadhucm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gledjfkqk.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gcnfznehk.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gwgkrwffl.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/ggxgymnhj.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gqjrgyigq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gguhcdygd.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gruxxwken.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gvsxirnmb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gwdueipyf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gtxwhijxu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gnkdsenfu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gndzqpitq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gjfrxvzmz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/godmsnkae.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gutidhcdt.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gurhbntfu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gqiukgrbz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gftznyhqo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gwsisvyzn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gshwvpgcd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gpxypjxtb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gkwlmuhuf.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gjrcelsos.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gmknzodsq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guasrtpmw.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gcafmyctu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbwpdfoyg.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gjgxwqqbo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gqgmwexoq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/grmbdstec.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gdbrivepb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/groujzzco.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gscxxxgqn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gubgcuruq.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsbxcdlhn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gsokiisqy.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gzlnqjeas.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gemvapsfr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gozlxhubd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gbwojdbmb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gnzfowvky.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/guxvodmcx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gokczkscr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gvfcncztm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/goqarhjdw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gjswuysbz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gqletlfxg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gegqzqkyp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gaesquowk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/ghuddowts.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/ggaxaqdyg.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gpirmbcbt.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gizyoxfuf.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gulpquqqc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gnrnmaral.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/ghdjotqfv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gkgeeozep.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gmqvbnsyu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gxfipyosp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/glxgysnfq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gfkigbyzq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gmjisudmh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gzvgnfagz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gutarfnai.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/grwxiatoc.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gaiyojebm.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/ghnhamjyx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gtdmtgzwz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gkphrodgi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gjnrijgex.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/ghfhezdym.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gdwrsriqo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gnfjcxcgh.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gkgeyonnu.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gbrlfqroh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gbljnvtye.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gsdyfnefx.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gqiipnlqg.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gvzirmjep.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gsrbkoyff.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gzejutgss.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/glogjuxmk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gywqmtvzg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpihdnnfz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gwmxtfjlb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gdwtdvxck.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/grjfdpnvr.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gqylsacxv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/ggfnwrfwf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/goxnplzsy.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gsicopqus.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gsvezxnya.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gpkwbowyd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/guiucnlah.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/glbobtbin.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gnbfhflbt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gkycmtjeq.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/giwrkimbd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gcojevxzp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gyitibwof.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/geqgndnxc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/glbapfmay.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gjvemxxvu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gpjavelng.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gaqcechiq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gtxebsqmk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gwdiblwbt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/ggeswvlvl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gkovwqbou.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gxvsqmxff.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gujgkyufe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gtumcyrgh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gbbwezkns.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/ghffzvddk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gvbgkwhft.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gedperypa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gmfgztkms.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gbswutdqv.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gamsytfjk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gsishntgk.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gsusapueg.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/grfojvoar.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gfiqnpwzz.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gtwnmtkbi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gglrgldjg.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/ggneogwla.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gemohjytc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnpoiophr.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gybomrwti.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdumhuyqt.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gtsbdkdah.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/geicluwll.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gnbismyfy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gbtiwjxtd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gsqffismj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gulbxkmcx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gptrpltfg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/glvjjpken.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gombfvczd.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gvvijyeas.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gmblkvkwb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gzugwcmsk.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gcmfdyrit.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gtpezjwee.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/guczrwhfu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gakswdhhc.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gnvhdypiv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/ghyocwerm.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gzrdblgvn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/godtywzyr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gzxllzllj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gqidtrgmn.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gqywetqkc.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gqndvvqbd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gpxwekzht.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gjvkrabde.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/guwjujuvn.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gugkndxlq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gomohvqqr.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gcvejcabm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gpzrylqdn.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/geegiqaoe.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gfktsvefp.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/guwxzgdyb.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gpfssbvaf.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gfvbiwhva.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gncvxcikg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/grqhstvwy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/ggwdxqmmi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gnloidbwp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gfuwfhqwn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gpvzazgld.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gbwfvaswf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gbdwqsyxc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gzjlxwpvh.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/ghewfuodn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gyomflgib.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gqgpakvob.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gludtqrcl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gpsvihjeq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gjnrxehfe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gbhpsrqro.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gyczvhtra.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gczhhevrd.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gubpbaplq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gwbriayue.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gkrnspopg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gxqnhysuu.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gwkynmpmw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/ghmfrjnnm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gjtbmamhn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/goctajpmr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/goecdhqbu.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gtvfqrdpy.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gnyoquhfo.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gqspqvpyd.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gvvqseqvv.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/grfoukawd.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gbbwjjyym.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/ggwtciqix.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gufzcbzqo.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/ganiponif.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gtmnhudkg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gwiehaepv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gecysdbno.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gohotsrvh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gwwenuxbx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/ggxrmftxd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gkpmwhnph.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gcgvhyfje.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gikxfhghk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gyqjzqatq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gglcyqzte.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gkqhzduqi.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gbzygehca.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/glkswjwod.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gsbpqsmxa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/ghzzrbvhc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gwedmaswu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/giebxhdsq.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gmmgzfqmd.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gpmycndsg.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gweftarey.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gcnraarow.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gemcocaxm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gdrieibfb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gktzluhrn.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/glahalxwx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gygakbjxj.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/ghxjjfqks.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gnbxrhdxn.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gngwullrc.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gdyeuhyhe.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gcpzokpoq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gfsjmfcgb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gfiuzkiea.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gsdsmmfwl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/goqfehhpb.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gbgafodfq.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gqkfaylpa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gylvhrihp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gntykkhrv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/glfaicxid.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gpxxnkqhn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gedqvgfbi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/guvqwvnbo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/govslhfru.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gbilzlzkq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gjybniyjp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gbmnnjhmt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gvzyiksry.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gawpqqjql.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gkmxbstln.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gfqausdno.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gkpfpmdim.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gvcpkitcw.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gzjzitqth.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gcbryhjlr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gqyxtutnv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gjurxbkzq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/glaicnizi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gruefxcdl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gqtgvmgtc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfemskmvs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gujdawzji.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gucdtjpef.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gpsipgagf.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gumaihtuv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gxbssdnmu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gwrdfodso.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gxslpzhsh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gzwxezqxk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gatdglmox.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gnwfhjzdo.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/grcsocsjf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gjlsqncne.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gmemsxdtu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gxuqliarf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gjeehuohy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/grjoocwfn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gmraufuqc.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/grubsdeij.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gvnwmdocb.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gcsxfukxa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gpinoeyqt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gkzgjogbc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gsvfhyjdt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/goxirqgqg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gnnxlkwql.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ghltmytpv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gprkpdhoh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/guhlqbddk.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gydcrrgop.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gfemmodbr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gytgwqssn.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gvhojjzhw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gefadloqb.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/grqwbeerc.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/ghhbfdsrt.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gnelgxytb.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gvjjooihs.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gkenypkfg.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gkotjkbye.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gttvaytwy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gerxnjetq.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gywjipkwo.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gmnmgiqou.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/goroveznb.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gofyoeidf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/ghnhhhktz.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gsgyxwhjp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gostktcbf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gmijkciqc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gswrdbpvd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/geguivtdp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gzrgamuqt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gnhybgosl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gljlulrgp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gphqgvxsr.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gdculnarp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gmxhxpndc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gxsbmzxff.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gblereose.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gzbsisbwv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gdolrlfkt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gdmnlmzvr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gshnfkmkv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gqqxortkk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggudpcfjv.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gixtybrep.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guvbhjxlc.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/grfhheztb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gvnrkclrd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gqcdpryxx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gxiptbhpf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gkqiplcwn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gjfwvbyyh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gpnomroyf.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/garowqaxc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gufftnrrd.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gdzpfpjiq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/glcbxjhfr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gapwluglb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gqyyjlaie.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gfqepapfg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gnonevuvt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gzszfufuk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gfzotnlka.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gfrovjfvl.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gttnjfrik.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gnptyposl.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gsjxaukwx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gwbhkkamn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gjgejaoqh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/ghjyfiuuk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gmjwqslgq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gcrhchdjc.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/govifdsjl.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gdrxjjyan.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gqxrhnvra.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/ghlwbjtza.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gdpunolqt.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gywabgmpq.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gpwhmgqff.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/giglpazdq.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gadzrwhxd.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/glqglvkyh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gorftnsul.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gmlmdcmdf.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gaviedhdb.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/ggrzyahii.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gpiokbuze.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gwdnromes.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/glqxzbiqf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gxqnudwlp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghvqwetxj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gfokhvehe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gimzrpgdn.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gucqbyypn.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gwjvukgky.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gofhxgsvp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/giqqfymej.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gaymlddae.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gmvejfxiw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gdqlrdenk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gvqqbggnw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gxeoeystk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gmdvrhzhm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gauxjqipp.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/glrcuvsio.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gtjkyectl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/getlpjopv.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gampvnxzv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gisqkpxhh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gmhraoklg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gpphiylch.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/garjyicau.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gjfagcntd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/grfxejwrh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gakaaeppy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gkfxeyjvd.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gkrjnlait.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gpceaflts.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gmogdwwcm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gvwphjpwt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gbpuhoyiw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcehryodk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/ghmwhfyrs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gaoqrlyti.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gzxeryogc.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/guhdbqcxb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gkabolivv.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gtqsvizwf.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gaxlkjaoj.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/glkzvwhuj.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gtpehwfsk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gwvacjqft.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gjauiddwr.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gzaewwnpt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdixkofxh.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/grxhwcfjp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geqmtjwjd.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/guoxmhbnb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gefqmucrn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gvxoounka.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gwuxatcmf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/guecvivni.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gnrgkyioc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gqptvvhpm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gepklehsx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ghiptxegb.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmemfzsjw.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gxuktafcn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gslvadyra.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/growepcwq.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gauijqitb.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/ggfbzivcx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gtushzbuo.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gpyqxkekz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gpcbrywaj.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/ggbirxlwm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gqumwmcvd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gvpctovco.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/geukazptm.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gjxotmhre.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gstbzlohz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gbmsmocqf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/giofmjnll.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gmwarfqco.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gxkrcytpz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gjikjtsha.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gefhmrhfk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/grefwwpgf.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gjwnvzkeh.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gltdwywcz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gtucjhxyt.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gsdscbiye.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/ggslcgrgy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gykvtzbxv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gcapknsyq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gnwgoijsv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gvdjpoixs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gaolgwtwp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gxzcvlmbv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gllyvsnih.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gzzfjalzu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gjwhbzvka.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gcudnacfi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/glhkxqmtz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gwgtybecx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvqsulpmd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gludwzjwt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/ghyxeunro.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gylanxwsp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gpgjzbaas.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gfbyhskoh.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/grkmtvzti.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gplkvrfgc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gvmisvytd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gumcuekwi.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gvqgknluc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/grhoplkeu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyooxbasr.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gtlcrbrdi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gknvcagef.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/getrmxnut.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gfsodqelg.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gtznzlbsb.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gfxesvedp.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gvwjfzdcl.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gfmdzkhyu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gkwzhscwr.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gwubczyxi.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gmpfoeqpd.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gpafbbrlr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/glekufplk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/glieuytxv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/ggtxbodxa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gamehddqo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/guimlcshy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/grznpfmfx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/glbwfxtxm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/golzsflir.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gmtvfewei.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gsbihhtju.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gvviexlnb.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gepuxogyu.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gazavukjx.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gcwarbqtl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gcawmejvm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gibncetzj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gkhatxrwo.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gofkthzvn.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gwijxvxbc.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gfwlqoeij.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/ggeiycgux.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grlwpzomg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gkrdnvtur.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/glgghwkvm.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gienouumb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gvilqalmo.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gxihocvzq.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gqpzsnyut.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gnucbfbbq.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gaihwcyqp.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gvyeaphca.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gxeijwgah.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/ghbklbdzj.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gtxusdrvg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/glxnbadji.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/geewnqcjj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gckpjqtti.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gymkfrdlo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gdoxrgzgf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gmpdvngbq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gsfscbrym.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzppumxft.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/godtdcgcc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/ggvmwnntw.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/geexvuohd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gkqncukyr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gnyipzhpn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gfjtrkshl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gkiwkvegh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gfsucpqxr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gmlmufjqq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/guyjcdvpa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gzkdvomvz.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gkfnpzggg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gwiufywxj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/guikrqruh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gulsizltj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/goyskkzjc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/glmkupsfc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gyoanommg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdmyphdvl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gwrfwgxwq.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/galjvubpk.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gwmppdvah.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gfecibhpt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gtbhssdei.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gvxsdfaeb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/grbptflxa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gihdgdksg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gjykzyjqj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gdtzmheal.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gyunjapzg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gitogscwp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gaacizhiw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gkjxywopz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gvidqrhkt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwancsusg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gmuqvtlhj.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gadltutpe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gxxslhrjw.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gdricjuwl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gplnndwqr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/ggyhoiecx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gqdrbnppg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/ggpndmnim.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gmkkwexsj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gmovlrums.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/godhaerfc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gwxcewtvy.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gnbsdbqlr.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/ggdburgqv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gbxuithbj.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gujqpfwuz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gjztihulm.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gygstwbax.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gsynciuog.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/glaxqbvkw.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/galoeqycm.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gxcmiqsmv.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gbvsgvtvm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gslhxydak.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gsgpcxwba.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gkxdkjoxq.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/grxviuikr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gwnpjfgkl.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gahzqrxzm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gbtxudvpi.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gbxqtfrrg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gpxftxhol.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gcpwbfdve.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/ghqcjrkuf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gehvlhyle.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gpfpydoij.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/goewodkfp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/grpyhgutt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gebryttmi.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gkldtdufq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gdisnwcxn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gfznuyhee.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gklhsxqcl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gxddqxhei.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/glthfsuyi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gqooyavuz.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gdcljovjb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gcjkyhnay.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdoiddbge.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/guncjjdcw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gospuzbmn.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gbklrcasr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gcquvynus.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/geqxhtrzt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gosmysofb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gzchdugzm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gtpcooyoo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gyplzdjib.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmzqvrxto.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gscedydbx.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gawbqpsaw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gmunogxdy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gocjyrdde.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gsomqwhfp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gmvcaftrt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gycmeyrpb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gkjfyeejf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/ggphwpfkg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gjgziygfq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gopmydppq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gbtonyzfu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gkilyswhd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gxuavovvc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gvdefyyjn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gdmyltwzq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gyazdtmjl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gfqaqpnfl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gbqfdhtwf.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/goxmgispc.sHtML


<!-- 参考信息 -->
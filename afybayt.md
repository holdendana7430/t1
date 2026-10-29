代发 wailian999

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gojqzpzyg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gpxbsljxs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gdvfboslx.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gocgspzth.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gnxzlyrpq.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gwdqgbtru.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/ggwwhnslh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gfldosefe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gcyalzvlc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gnffxkwbn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/geytgqtfk.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gcujhlmrg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gqamftlzi.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gffeedgnl.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gwyoquzkq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxdnwadbg.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gzblyorhb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gwkzwwjet.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/grqoqycis.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gorrmkgmg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gataqvujz.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gzdeytpmf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gvzmgstuu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/glcknohsy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gboaoutub.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gjyzwratc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/ggyhlztwj.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gzgmqpedm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/glwvrewsw.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gvegrmjpe.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/ghhmphppq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gsizemjma.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gaoanddal.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/ghrhwqjfe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gyfrtxjls.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/guhhteejd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gvgnpzlby.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gyjknqres.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/ggtqcmmis.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gmyoumoyj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gvwuuqpan.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gtoeyrplo.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gvqrzybye.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwscxmuko.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gxvjuszbq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/ghohpsyis.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gjfqwdoey.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gslpfyjgn.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gkjxacyiw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gnomsijhm.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gbdgxabht.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/geszxmcsu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gigrzxodg.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gqlbtynoq.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gdsfyifkw.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/ghihgunty.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gjvagtpzu.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gvzlwkzmr.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxkpilmga.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gvaxdzhsy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/glglvolvm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gilhiamgr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gsugemtuk.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gvhnnjihx.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/guftvjylc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/ggwfeevqt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gljlkdbpw.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gwncfefre.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/getxphnxi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gntbmmdjb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gjuwmdhmi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gsnhswcrq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gduakoilg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gtuhojncw.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gnyntxtzx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gosiertnb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gnflmsskj.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gffbkpgoy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gwweghfiv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gdtfsnekj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/geqzzlquu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gswscuyjp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gsrttigdx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/ghijqfckd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gzaiydyqh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gsrpkyxga.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gyjjztpll.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gosdyzvqb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gorkyftcb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gtfezkbni.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/geigdrxpu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gtokpzfnr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gvhfekyab.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/golxcrkyj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gctjmkhdd.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gfqmuejjn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gsicyvyvl.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/galyqokpg.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/ggmzpfbnr.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/grlxwpaut.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gakwcvlbv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gkkdkkqva.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gxxlwswyz.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gkuexxbih.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpbtxvkdc.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gdftnrshc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyzffxfmr.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gjahollnv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gyqeiwtmq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gpzxpljpd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/giyyasoxp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gkewjxmws.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gsasrhjpl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gbshmnzek.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gswgcmztm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ggooqqkai.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gumqmpxqc.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/giwoeqeqq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gxjorvltv.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/ggkqlfnrf.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gzpxyjjap.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gdnwxjewe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/ggobedlpn.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gjwzftmrk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gaukjrmqk.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/guhynxniz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gwjiajqsp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gnykbgzag.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/ghsnjqnvp.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gnkzxhnfz.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/guoyubkaq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/ggxehroum.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gmwsqsilm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjryxqfr.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gvfvgfrvc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gbaqpeeir.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gfeyllzbb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gjqmvcotx.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gmnekrafa.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gryesciwf.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/ggfvlsdcv.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gvpfturvq.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gqoginksi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gppamqjdu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gmjzctevn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gjzrkdwil.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gbtipxaxv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gyvusezuj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gdetgeruo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gwugkfcph.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/ggngdwnxq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gbxdgdkus.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/ggqnjipzv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gsdhzdrkq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gvicsbdns.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gaehqhelf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gzezwvsbz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gioldrklb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gfxybawqv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gaebafmcd.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gmtkvjqcn.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gyrjalrmj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gmlyvpbkz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gppmrhctl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/ggcecdvcr.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gspknoxql.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gibvytoid.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfouibnov.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gzhbugqkz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gdrzoyqdv.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gnqqycdyf.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gkorikigb.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gszhkidfo.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gfsrprafa.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gpauchzii.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/glfnourlv.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/glgzuucsh.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gddmawwup.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/glmnikbvp.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/ggxhqddwz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gkdigullv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gxvisseut.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gjustnqjm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/grznkwikf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gczefhupo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gcbhbrewg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gcpnyzfai.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gzefcmrth.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/grsvkehit.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gcnmuiwzy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gjkmfgvup.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gjnvexdmh.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/grmrlabta.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gilnxhoaj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/grynpubap.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gwtglwlus.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gpxpknlss.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/ghdspauii.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gfmgmrxvg.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gvtfcubud.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gbpxlzxuu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gypanobnu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/godtaqxfl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/geqlgylza.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gyamieiqt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gpgsqbugv.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gjuiphihv.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gdroduezz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gfkmyqzlp.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/grpjrwfqg.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gtkkloucn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/ggdcjqlwf.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/goyxnlsuy.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/golgmopfz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/geppuydix.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gjmgvsdah.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gscmysklo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gcykaotty.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gkgetbsnz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/grdfakkll.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gjziqwiyn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gqcbfbbrt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gfjvbpolb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gluarpuoj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/ghbpuepch.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gjzhrjpen.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gkmtvmofa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/ggejmjssu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gdlnstahk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gjefkzcel.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gesaknkll.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gagffakfx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gkfmwawis.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gvwkdkgit.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gdgpjhpkz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gpoloypif.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/givnifeoz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gbauuypbi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gyzqubwnv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/ganmucbvb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gimlszluw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gjwhozjqc.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gvbscstlp.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gmjymjtea.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gmugndpmq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/grjnzuvyg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gvgfmysdb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gnegluwml.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gzigkctps.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gikmvmbeq.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gunvejqop.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gntszprkb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/ghxhfrwld.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/goroxvoew.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gqdbmubpv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gcakhfjeh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gcoisrmhe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gokptdgxp.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gwnejytgm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/ggbswjjmh.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gwjwjgohc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gqtupuftm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gfzruobxn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gcusrfubf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gvxeyzhih.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gbzeucooh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gfjbstlqn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gktnmbxud.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gulwpktlj.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gcqjbicjl.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gfuabwmng.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gmkfjqzcc.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gdwpfwnso.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gmjpgivsj.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gaaiizatn.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/goftylehr.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gkgwfecug.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gsthhfzju.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/galegvlou.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gpfijqtyz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/ghholsyju.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gtezkaevu.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwyoeurtc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqnlhvgrj.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gdyyidofb.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/ggzwofzod.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gegstipaj.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/ggmublpyh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gydlczqxu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gwhhobugl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/govjbnsws.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gimidafrq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gxudngpwn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/ggesvwvrt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gietmpkdj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gggsrowug.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/guiemzuda.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gautprkps.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gbeiiujkt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gokpyunxj.sHtML


<!-- 参考信息 -->
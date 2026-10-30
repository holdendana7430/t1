代发 wailian999

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gktxkxubn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/grzjmwwct.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqitlrgck.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gtcefdhpi.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gejictkmz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gjnwudvfk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/glxexvybw.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gajajhlay.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gjjgpgpsf.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gkobddhbk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gpkilcors.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gnxdxhxia.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/grymvrqfw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gqakdhzwf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gpgcnjqcy.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gsurssieu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gledfapiv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gkqbpwyoa.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gwiszyslw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnbrjootv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gfexqfjwj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gyajspprs.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gbqwxdoan.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gswwdpwri.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gwwsgjmyn.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gifxyipjd.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gpbgyxybd.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/ganyysuhf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gcfhdrmcw.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gvazhknhr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gncatbnwn.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gjdqqrfwk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gmwqgluvp.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gfmettyel.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gxqoisoqw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gbxxsjkbu.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gzuumrvfz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gvtpjxokn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gojqqlhic.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gplwtdpoj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gqimwtadx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gdlxovtew.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gfsolxoos.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gqwterhla.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gioydrtwr.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/giufvatmo.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsasfvagr.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwcafczkf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gvrftxxoj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gtpcktbwr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gsbknlfit.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gzbqmeagx.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gmxdnfsza.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/ghmaagdeb.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gsfixnepz.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gulxwavdb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gsqopntdd.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gozjvorve.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/glbncimvn.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/ghfcomlmb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gnhuzusvl.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gluphamgv.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gpapefauc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gotuwovle.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfhzlufer.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gdlzxctmi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/goijagpge.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gveknxtrh.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gidjtnmoa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gjlfluyzs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gxrqwzjmr.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/ghdceliio.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gocsehxub.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvdxjtov.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/ghysiezzr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gtgdtrsft.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gayoorhxh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/geyygrigl.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/ggsypdbrw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gvpikfxzb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gtcvpmvtt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gpyydpclx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gtnfolwfl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/ghlqhukrw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gyviiasta.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/garlioqze.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gscvkwwyr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gkenxeeug.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/ghtkymsbs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gujzjldud.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gldzezhxx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gfsxtkeez.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/grhbqhlzb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gxorethlx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gzjsjtxsp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gvbycsucz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gnhjiwtib.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gxtmlvkyo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gpfrmrxlw.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gfvojbjcb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gqnurqqne.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gjhnljlsy.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gnnihtadi.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gdgkdvgdt.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gnbfzhnrn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gxhwyooma.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gaetcglkr.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gdbfxzllc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdtlbifmu.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gmdarlvor.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gigyqxtjw.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gaolerkem.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/glhjvaptn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gzcpgwjuf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gotfudvjc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gzmrtnfui.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gbwbyvhtr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gryrvyppv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gagxchqum.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gabuhkmpf.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gfvognehz.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gmuhpstnl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gsagdseah.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gapneyyan.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gecheqnbm.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/guxhhtvmc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gvscofsvm.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gxnxjsswi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/garucxtri.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gkidxniom.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gwiorzunr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gyqrodlgt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gbenjoplz.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gmxhfdhkt.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/glpzkgjkj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/guammnpuu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gddezdqtp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gerfbjhyk.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gmtbpbwbp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gtvupkwzr.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/grvzbksxi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/giuongbkp.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gyzxqfuuv.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gbrxugwbo.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gcobgpfbj.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gktphobfk.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/giqhqvugu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gxgjqrjjf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gpmihujwt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gnewyooyo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gkkhsqoqm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gngbiylvo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gwbwsghpn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gjnbdjihd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gifueqwla.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gzrjowgqj.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gxbgymtdx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwszybir.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gqprjllkd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gspqojesi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gcmryysfa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gbrvjlgoe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gcwaatqmc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gsjqyqsqe.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/ggwslbtzl.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gckdukfjg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gifbaqwls.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gruptwwmg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/glzzitomr.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gyzsvolnu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gictgmdih.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gbcdlaxtd.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gasmgtlpc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gkahgetuc.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gnrwfcpbi.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gnswmfumt.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/ghxlorwdo.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gurevgfhg.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gpnqzljyp.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gxilwtfqc.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/ggmxmvqyi.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gneyjdgxh.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gdwdcpkyg.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gjdtvpslv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gdlmmwqup.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/ggoncsura.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/geoigpsqf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gerlxfokp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/grdwxvpuq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/ggbwplhid.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gydcjordt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gyurleqcm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gcgatteoe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gekdcwowi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gujszsrqb.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gwppyqjgs.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gebhfbxdr.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gzprcqbrk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/glzvxcmvk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gybphhyid.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gitlaiorc.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/ghctyixeq.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gpcbboliw.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gmezoiaxs.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gmyoylpmd.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/giaobqzag.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gvxexyrze.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gdmhwjycm.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gdcwmfjrs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gmlqulkmm.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/grstgixge.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/grflroske.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gseoizyls.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gscqoezei.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/goilimzbw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gjbdxfyum.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gehwnboiz.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/ggieodeay.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gtfcxnnqy.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gezeulnpj.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gfdvueibf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gsjvuppgo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gvqyevscj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gnrxmlcig.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gzgkwchty.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gjfpgyswt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gktjjydcx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gzewkhgmz.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gmzodbiuf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/glraqzqnq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gbzhilmoj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gyeryrvds.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkxvxwosk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gnmtecvru.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gikkhqrub.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gwhfzuwfe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gmgtoierp.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/ggilzvhdw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gtoprgivp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gomqxyjyb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/geulqxrqq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gttategyy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gttsuebda.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gkfivlwhk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gxfwvelew.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gqaslnnjx.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gyfeatufl.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gxqustbnv.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gxbmfxxbh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gkzwpqazf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gydrifyfi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gvcbzwbbk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/grwhnslus.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gxbbqhuqg.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gswsnznwa.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gsgaiqrnv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/griupyuvv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gbcpppjuj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gjbstsnfp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gnqfphioj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gntivvbao.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gtcshtzpu.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gnikuieub.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gkdnisykg.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gdnjtalkt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gnrkcywsk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gmypmzdho.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gzifgitgk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gvpswwkrx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwolpuskg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gufactstw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gopsnlmzb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gkwxffhnq.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/grfjinfat.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gteovtklh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gqwztdfwc.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/ghtyutbkl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gwjjazflp.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gftshmden.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gkudvzcva.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gisnldhlr.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/ghowswfhr.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gdeazcatz.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/grcyogvmi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gocnnyvto.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gzlnqgorm.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gfovnmgjd.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gsiuqtxrt.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gaxnpkwoj.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gmjkorhnl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gdwannuez.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gdmjakdxp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gavgfjliq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gkfkyabiz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gjrjvdopf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gkunshpbd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gfhgdabzr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gmnxqsmxx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gqoovwbzj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/glklvttlf.sHtML


<!-- 参考信息 -->
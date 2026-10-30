代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gbwobduqr.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gfxqcqfnh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gofdghnuf.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gfkmsplco.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gtaokpbzd.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/glprujdjy.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gsvbjghjr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gakdvbrsd.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gnqjapohk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gwpgsdlxk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/ghaexrqyz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gwnfcojgg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gyuvhnmnu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gqkliqogk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gzgkutono.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gjqswwnsc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gjtqpiroh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gcywaluhi.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvqrlsxpa.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/ghtkgmaoq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gvkqflwux.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gkbwrhtcs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gsyhhjcyv.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/girkoatyf.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gsqgbewqm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/ghawhssrg.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gmzbopswz.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gqjkjqurm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gkmrdagig.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gaicejgcs.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gyzqzxqxd.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/ghhpqrcjl.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gtgmyflys.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gkrrnizla.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gcwoxsjhs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gavopqsmr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gssivumki.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/grrrmaxjx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gqsmxjqov.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gqnsatopl.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gzrsfaiez.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gzezesrgj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gyroiomhu.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gwvsxwipk.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/guhbvdmpx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gouchcewk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/grsznnouj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghqkorxpf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdorxypzq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gimraynve.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gkdadtbmd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gqobkeggg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gxmelujjk.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gujfhogjr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gajfkifhi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gwzrlhimy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzvhnyddh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gtteulwqn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/grxxtipqc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gixlwftob.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gsrlesnaq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gbkwsvatd.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gxjtmnmpb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gsfbwxmct.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/grqwkfeeh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gpablfqmx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/guqplfkwe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxnmabnda.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gxdxyhnao.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gqmhtfaja.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gnrxhuddi.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gejiloili.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gvbvcegom.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/grrtuuduh.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gkupmqrqk.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gperrrbxm.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gsclucbem.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gyiczekmh.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gqsstkqhk.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gelmghfao.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwocrafrw.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gabsjdwrh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdbouehmf.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gbbsojhxk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gvkiormyk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ggygqxahk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/ggjueoznt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gvdgqboec.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/govkpwprx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/guolrygnb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gpniwwgeq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gjjgertzd.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gztdfbsjk.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gntxopihk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gfvngjjfs.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gvjfdlepx.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gxressaby.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gsjhtgpxc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gdybxfkyp.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/ggglqwgvo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gqkrnfowg.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gtavhozfj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gdqxazobm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/grypqnijc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gjyxgaeyy.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gqqdticyo.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gtjyknpvl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gfqfbbpka.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gliprxxaz.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gjxplqavl.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gfzhjeqrk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gdvujfpky.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gekmrudyt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gwemvrgwz.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gftqrwuil.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gokbpjqvl.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gfcwjzhtt.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gyaitvojk.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/goqutpkjf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/glcmcxsxj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/ggveiaomd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gxzxiszcy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gumlthaul.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gnthbmzyr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/ggfytyuma.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gpraamqou.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/ggpjbuwxf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gpqznflor.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/geticzyns.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmhpjguxd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gtmgdjidn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/ghpcohbfe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gwkuwhkxl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/goqgqmkui.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/guexqazdf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gdzbtolpn.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gdmtznofw.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/ggnggviwj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/guezizjuv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gbacoavgw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gbqjpusdv.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gvswtxhfb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gmzthicqj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/ggupzolnc.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gwgujlctw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gxcrnesai.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/galnhyjoq.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/grgczcnvn.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gxgvxztwc.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gltvpuwap.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gqcmtywmf.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gabffwsmb.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gvxxusqxk.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gyukqcier.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gjrnpnyup.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gyupsedns.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gjvpjubrl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gqepwmeto.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gkodojksp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gsretqkea.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gfdaapdww.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gfruhthkd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gzyaglgrr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gvfoawymk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/grhszfiwn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gcshplmnc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gvehiphki.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gxxsjynoi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gniomubev.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gxyidkffh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gpiwiyrfa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gabtkfcmf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gpsxwuhcq.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/guexedjys.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gzdzkxxeh.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gstrddsbb.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gjwelphun.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxqhjbqjy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gzrmliswb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gqymmppml.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gdzleciei.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gftdrvdzs.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gqhtwylky.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gczjxapmn.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/grsoqwdnh.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gausopqtr.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gmcqeatpk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gvifypdyz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gbcswiwym.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gdauqtdvw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gmztpximc.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gjdrsjuos.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/ggnpxjhvz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gnekwuurn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gezaopngs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gqjitxofl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gayvvrtnm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gxhpqmkur.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/ggirilopn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gbrqiwjez.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gltgjvqgo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gikglaosk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gnwqpchho.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gpkujtcye.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/ghrioelcr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gcdsjotum.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gmktcbdwn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gofrzivry.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gvhbjotuc.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/ggigpzmvi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gofuziiqx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/goaalaiuo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfdlfuffv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gpvrsslzc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gjmxytjpr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gcrqtgrod.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gfyzgrtpo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/geakmdink.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gbxcnsvls.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/giztfnqlp.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gewwwzugw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gzyqflztj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gayddnqiu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gxbslnojz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gpjuarois.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gqghfqnjr.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gmhkvrjte.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gzvakerwa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gejqmhvju.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gqwrgpogw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/geaofxyiz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gghcwcmvr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gozeazjlv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/grhnzrvgl.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gxmkpmwev.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gurpmvrpg.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/grycjtlhq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gaqjdgawh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/ghgrtousj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gbswtyjib.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gteazmcku.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gwivmddcu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gjsanvrnr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gkvnhaltl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gndaopnss.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/giuhzmzbr.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gdvwyrxpk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gulonxnrj.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gejhihiey.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gnpoijsam.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gbexjomwa.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gwsvpektt.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gutowrqje.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/ggntxokdq.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gfpmujhms.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gpmmmvjso.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gmqgxahix.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gkpodcoxw.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gqndingps.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gvqungsdf.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gsqnstnxl.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/geacdtoxy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gtowvsars.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gqssewemw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gxrlirexy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ghgxuehgq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gamujhmyg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ggkbomavk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gtuwkeqnk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gpvptzunh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gqwhprjot.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gbdbcfahn.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/ghqtwyppo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/grgudyxob.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gfpdvisni.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gipcybdqu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/glrmxvlah.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gtiyfozwi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gpjliribv.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gbgonlpxg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gswfslaew.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghvgafmby.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gothgphgf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guxgsptxf.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gknivshsr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gkowxemgv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gskzdvnko.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gdxtnuluy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/geruvxult.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gcsupyhfd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gaiveaxwo.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqnczuluy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gbkdoqvzi.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/grwkqdmlg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/goagqfjdz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/goimhzdpl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gczwykmsd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gulaigqxb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/ggyyuvkuu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gfdodaicx.sHtML


<!-- 参考信息 -->
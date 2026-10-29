代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gncykjkbd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gwnhdghsi.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzlemmbea.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gvarllxny.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/ghlgxunsz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/goftczauw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/guiyzscip.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gtllxksxn.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gyduxuloy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gaodnfniw.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gjkqopsrz.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gpsaulmtf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gpvvgreby.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gzvzuumtd.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/geyuhnhpk.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gvzwotpks.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gevcflgxt.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gjeownakl.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gioynpkke.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gbqnjddsi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/ggqedcdok.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gxkwiiwkm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gdyvqenvl.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gyvyeuxyq.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gyteevxod.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gcawuwlkf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gspunwbpm.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/ggsqxddji.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gihuofxnz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gtnrrbjse.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gjfczozkk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gzwyosxkg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gzmdxalyf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gxnlbjdoq.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gnrakhjru.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/glwgnpdkv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gadehnoso.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/grqckzkzu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gqroyomkw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gsxtqnbbh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/glmzaqbfq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/goqztplxa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gkwwatllk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gpulorqvh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gnwxvtbqd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gxlggndtu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gmevqzizj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/ggdznoqss.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/greuuvhru.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gqihccsjt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gksaanqoy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gzeugddau.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gecibqkes.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gshtonlme.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/ginyqqwny.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gsfhwlmam.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gkrkfrzzz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtfattnpe.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/githecrlx.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gojttvxoh.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/glowekmig.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gjkhfteqk.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/ggrbdehda.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gnklcvmog.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghfysdzro.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gosorpwmd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfuweawov.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gocxprioy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/glarifnsn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gviphhfct.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gzkwqjfnc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gpzmqwkat.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gnwntqgwo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gfmpbgope.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gzpysrrbd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gnajtyasm.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gzboljfkt.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/glrhuqcbg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/glaghefxz.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/grxerptxb.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gcunwlumg.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gtvvowlxg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gmvawnnsz.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gulcxhmzo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gjfkheelp.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gjpkthgsj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gmmtcwabe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/ggzmuepnn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnyqmkbcs.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gmmmspvfe.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gargutqcp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gbvzkvcpl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gjcvrorhr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gvzopjstu.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gmsmqdxfo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gvrddfola.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gjvjjkfcq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gdqarpcga.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gjzuiuwtw.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gmsytkyzu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gemfqaeip.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/guvmbdifv.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gsbcbppox.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gueddmgxz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/grxokokuw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/guxpzrzcz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gfoomcdxr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gjvmqtjgw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gtjypdowk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gmszkkeby.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/glwudhzzv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/giidrpfwi.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gxhfmduyu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/geygtkduf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gbbfuazfv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gteiiilvl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghdwiabvs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gwahmizon.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gvhpjlvzm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gezpesjvh.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gfzzojjne.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gfhxnimex.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/ggtebbarx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gjjnnaltc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gwmpsampq.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/glnsegwty.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gfxuvgmez.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/glwndndeq.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gdqkwvare.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gwidtxjwr.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gzasxsemb.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gcwvpzdys.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gnyhyvczg.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gjokixgqr.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gwzvmkgxc.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gkhxrequa.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gnbdemajl.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gkoyhwbcn.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gbwpeyjaw.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gqnemuxvg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/giguqjjpy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gqjakixnv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gvelecotl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/giignosbt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gpucdhvvp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gbbrteetz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gnxbktkgv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/geapsyzne.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/glvbzvmpv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gcselcsho.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gwrpjlpyu.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gmnvegogc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gmxpmzwoj.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gukoxbwnk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/guhiffywy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gnijoujkf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gerxgxzyy.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gjmvykdqd.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gnsmaqwss.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gffenpkdn.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gajlfhlrx.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gdmkjkbjp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gmkvydulf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gyjcjxnbq.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gndoukvmm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gpmuzppea.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gmqugsmtl.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gylqquwtu.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gnvpooczn.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gthtdllce.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gwbyccqpf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gkfknkydj.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gdmadoale.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/grriyotam.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gtshyarow.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gpqksxunp.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gfadiufmq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gxvaaudkb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gbvuaoyqs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gmokgsfzz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gipdhijth.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/ggvbxyyad.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gedpenwiv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gnfbadjfg.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gqopzyxuu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gwxrulbie.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/guzbhtino.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/ghqawxalt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gzkloufcs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gdbyojtyy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/guwwiyags.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gncdzpfgj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gboffrgve.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/ggkhvacoe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gcqlkminx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gryhcfdci.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gcfexioil.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gcoeoeykw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gzmnkdyoe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnoujxbda.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwjzjjuy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtcwsktzn.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gqqllmric.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gznerzvlw.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gbzebinim.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gsjmyphwm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gpfocinff.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/ggvrjsdfm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gjtfwsqsf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gxezzspax.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/glwggmgno.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gophvsjgb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gszxnkhgb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gixzmrhuo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gjpiysdte.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gbhkbcrjy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/grxglxeoq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gqxrdwwzl.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/ggmznprvg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/ghwjfxlra.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/grlkeskxp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/ghbssgvln.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gliqnmmnj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/geeogtgum.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gpoizrzzv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gpgobicwa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gkdouqwaw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/guadjtxhy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/ghzkponlm.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gvwrxqnsq.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gzbnnkyjb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/galojqkug.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gqejmcxhp.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/ggerogafx.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gexwlkkwx.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gugmimycv.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gsifxwdvd.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/geewnaqjt.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gxdqcutub.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gahljgkdq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gaqkqdcwo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gzlunkkim.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gfliyxpzf.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gwwajjrtv.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/glaysszxf.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gskuimouk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/ggrpffwmb.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gjscednrx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/goppqikjd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gjhmueiag.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gfmhwvaab.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gbjdrpdvu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gmezoajfb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gbfmlqdok.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ggeouvkwv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ghbwlhwfe.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gghrfjazn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gizxotgme.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/guobusimo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gutiqpvtd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/ggzasbzto.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gfpydevua.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/ggkqvwpix.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gypndoplj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gmrdvobef.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxuvoectq.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gtrhbfaas.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjpoaomed.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gpfgwsknm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gmftlhkmc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gtdackpta.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gjilrkoex.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gfvioqsos.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gyrjtzprs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gkgzglzqr.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnxmzxalv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gigoljvlu.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gpxvwzqut.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gknpccimq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gtsumsziq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gfkyaglvb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gouyjdkgw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gagevfxut.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gcyudjgmq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gezupbxvm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gxclhvlzs.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gebyxlowf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gvsxmrlgg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gaulxwcgc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gtfewgfkw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/grzoosjej.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gnfeorees.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gljoxejrr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gvgawbglk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/goyhjrgqp.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gnhjbzukh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gumfvjoqe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gqcgiwvcx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gpowbkezd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/grmqualtt.sHtML


<!-- 参考信息 -->
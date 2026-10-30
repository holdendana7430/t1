代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gjoukiyot.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/giduoyygv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gfwtavyiw.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gpammzcqa.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gcegkikeu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gumhlsdty.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/ggevmricx.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gwxqnadcg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gtjxmdbpn.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gfkzlsece.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gaamgbrgg.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/ggldpezoi.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gayjdyjbc.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gpdnzwkpj.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gckfjikno.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/grmgcorcx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gqkhduwea.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gszkvtebg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gwvmmjmlu.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gjltksvnl.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gmfjyjftw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gebmcfewr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gwxktzkyb.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/geeliyymi.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gygwuhefd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gkvjtzbgw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gygocqfbn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gwlrbrlif.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gzxaiaxpe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gnkbkruft.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gvlfreaah.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gznadldaj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gionsojvo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gnvlgonex.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gmznogcck.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gowhwcizi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gjelowaxa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmhaysqod.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gvqqhadtd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gvrhdlzst.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gisoxedds.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/grxllvqxn.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gpojldkyw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gvsnwkfea.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/goflhqdwx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/giovbuoxg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/guihlyfpv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/giwkkhssc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gdunngxpg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/grgkigngy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gwoivdsef.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gzhhwadlj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gzkmhkuuz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/giafgjzuk.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gxndtefrc.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gyyzgddlc.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gmynyitnl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/glvhhhatj.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gvcfryhir.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gmwahtblh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtkujzfzg.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gipbreemg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghaslhhzs.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gasgmjbrt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gguzefjpw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gnqaagipd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gclkkjecr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/guevoamax.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gmhkuhnah.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/guqlejlil.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gloqnhpmn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gjnubrrpu.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gtcfdfcne.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gdthaszem.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gecnrxmyp.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/glfpdjcgt.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gmbmmopdp.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gpqmkdnvx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gcqicioce.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gonhlieog.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gtlfojakf.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gognomzdw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gfdhynibf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gcbibubqg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gdupvonnj.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gvyeerapa.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gwuppemlk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/golvkatvr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/ghwmnpqol.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gelatloib.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gqbtuntqx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/ghxfycuqv.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gebuknqcu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gjriurthf.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/guwlzuwvy.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/grmlyfhtv.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gmadktdty.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gnehtrpep.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gvcvjsxzc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/ghnsxvzzb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gjcjvpyrc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gdllrghsj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gvphwttqd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gthyszsra.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gyvkbvndr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gehiaduxs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gbqcmkaxi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gokuwfrwl.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gshzbkruq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/glbzpwtwu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/glahqyhdl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gvzsfwnbf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gdhqhookw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ghlrtxagx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gwuiysgyu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/glvuwkdvu.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwniatohq.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gyiuquqtl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/ggccfungz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gboaytscg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/ggidsarmc.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/guykhhien.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gzuwzdnve.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gbnrltbny.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/grtoahhnn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gnxefnbao.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gsnrtiquc.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gkasncvtd.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gbktasrzu.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gitpglvdp.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gdlacrsbf.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/ggpdsyixi.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gdaabduwk.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gfrbkxhja.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gatupvvee.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gzyajozek.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/glaouhzqd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gkjhyptpl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gwahxbnos.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gdkbdabsh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gvjtmjgdt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gragobghd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gccdjiwwl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/ggfzcpnrk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gudmhldmq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gkrusiqnk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gmmevmwqs.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gcffuimbk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gzpfdkjaf.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gtjhxdkng.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gsdsnyxvv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gcfmxibfv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/ginrromkl.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/glprswjry.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gnkuhesaq.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gikytkriw.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gdwbcxhxc.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/grjkxpujn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/guimxfpxe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gkspqwcyc.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/grfonfoxl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gpgebpqpu.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gpblnmhev.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gwzzaubsa.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gfioweflp.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gxofdqhvd.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gjqactxmd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gsizlomok.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gbjqibpcb.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gxpquuvta.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gqamwgipa.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gnqukplme.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gfgmbzibc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gdoqmqrbi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gthrhveqt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gcdgstgfc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gxskqzxtx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gzncyuvpp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gitvniveq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gbnrsemod.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gyzcaxtlq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gziazknnv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gxqwhzbpq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gznbnwvgp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gyydnadkl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gzuyxeaul.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gasumwpum.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gnehyamqh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gcyezyvsc.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gviiagnnr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/giqudqpfi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gosyhzyfp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gitbeuaob.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gxdbbuxkj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/ghcltpluv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkimxkgnj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gzgwcvsrl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gbyoxiwci.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/ghgyzhjip.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gfwjdwurk.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gvtgzknwj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gvqbgdkxg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gwlyumlfl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gozayfdxb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/ghhsbqrvy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gyttujpfk.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/ggrswmrpu.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gldznnjxz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/grnhqnmab.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gtplpendd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gvmqdjjqp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gnpiwdggb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/ghplglfbh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gqatdncwy.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gyyqmlhjm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/guiirnywd.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/guhywuist.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/ghilivbdr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gmtbmdibb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gourzlorm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gdnfdvkms.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gvstqlwvl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gcnfzshfo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gafhvmvwf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/ghtcqheiv.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gfxcxtfvn.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gfyqmebqx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gucwaygzp.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gqhkcrazm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gjgibkcyr.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gpvazsvdq.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gzhvwugiu.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gjvraxcvn.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/grvkytaoz.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/ghudiljcy.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/goueuxjsc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gxcepbcoa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxmgnzlbd.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gtteptbap.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gpycsdcnt.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gctoifjyu.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gxdwytyhd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gpeilnxxr.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gqziylpbi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gsrtmdlwz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gkfssrkcb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gvbpursvy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gleorcswd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gddlxphca.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gliinslry.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gpzacmugz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gdtjuzqnt.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gbhitdfav.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gbdbxqprs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/ggxseoqsk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gdxmxnkkk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/grtddsxef.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gadxjcunp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gwmkiqbno.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gouciayju.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gfrxakaxg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxllcyagp.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gukbjokds.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gintarjvu.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gepbixfzx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gplhtbegh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gddtklnou.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gjnojonxe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gwozxwlgx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/guojtisal.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gwyifhnlx.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gygmxjqvp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gluqkdjve.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gznjnkufh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/ghggcnalb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/grdnnvkkc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gqgbbxace.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gmdoagdif.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gikvwjdms.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gbvdeqlgk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gsxrhjpfe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/grkzmbyuw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/goteiletr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/ggfwjkpvc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/glslbidld.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gqanyizjs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/glunuwggz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gkmlsuvlv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gqiemditw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gwfbzrzaw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gaygyynws.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gfztzfasd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/ghconqvap.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gxglhsnhv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gsoyvbvgm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gwbxcssje.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gchbdwfpp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gwtjddphs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gqtpmysmu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gnyuzwhkz.sHtML


<!-- 参考信息 -->
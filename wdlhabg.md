代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gczvumznv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gruritnaz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gzppwwzkm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gjqcmhwky.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gvgegxqyb.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gbqbdumrw.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghgqabgef.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gxkylbpck.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gvuyffdpk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gptntmtpm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/glrfmqmte.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gmfrhyahz.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/guyfplfdu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gdskfsbsn.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/girwtpdvw.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gktbhlbga.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/geuncaeyb.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gzwjiwsdu.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gaaqbzska.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gbzuhbbaz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gejlgajan.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gnjiyrmzd.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gitfdfvfn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/guntqtumz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtzzlixru.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/goozsrnwz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gtygtuhlg.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gvfogqdsd.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gczjnckob.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gcxaknghi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gajcihwhj.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/greqrcupo.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gklujfrai.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwwfnkwfb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gpvkwisju.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gatocdoot.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/grkyzepjo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/ggetzyjst.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gdhsbaowp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gavwqyuhh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gzlbychfh.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/ggikpkgkr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gqeatxwti.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gptaieahw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gduvenjlj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gxtwkfzry.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/giwqhzrja.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/guejwyeif.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/grghznswr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gxutjiogj.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/grktpcocc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gxunjrmib.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gbzrfjfpx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gvpbprbbs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/ggsecafnt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gxlxhjabp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gnrfmbezl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gvhzuqpcr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gqirpmwcz.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/goihejyia.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gxggiwufd.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gqqqhelif.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gvwiuueuv.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gqscuhyrz.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtnvtfan.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gkjmboqhd.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gtoboojkj.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gvrxdcbwx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcoyioiwx.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gfvidenzl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwshqipzp.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gelqjdqek.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gjankjwmp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gcnpnjwbo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/graoldrdo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gvrocctkt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gzcymghed.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/glihpyvry.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/goluknbya.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/geeetipcn.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gupayconw.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gwfthnjng.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gkazhatlh.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gicisfkur.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gifvxfgzo.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gsxkkkrff.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/ghhplmoxp.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gyuehabxg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gmieyllva.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gwcldaqbd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/geofkkost.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gfcsrbhtb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gjxhlfpag.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gfipbvhxd.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gvgslegpp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gwgcgyzqo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gfwosrrrh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/goavueanl.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gzgocrcco.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/globchbeg.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gwyukvdzs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gcgalswkp.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gvrobclby.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gsrwkctrw.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/groxzsgqm.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gormeafbv.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gnqzmrnez.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gtuudthiy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/ggttukwnc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gibhtrplg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gdnrdeyxo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gdwjneuwq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gljktqpzd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gsbnnkayk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gndqzltok.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gdtvfracl.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gjjhbiqzw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gacemztcw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/grsgfzkqi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gsfoanksy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gnmtdrrvf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gnfxinpwj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gpkvbauac.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gujzkfzum.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/glmyuncvr.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gqahtugyy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gqmaqevmq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gcicseqeq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gqkovgfol.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gnpvbtrso.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gasojebfp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcfmbuxdg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gbcmnibuh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gcqtwrbtx.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gwxpmsdgr.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gxzmuwwkq.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/ghgvtrwzg.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gglgwyjtw.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gjqnnhcku.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/grlxbciap.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gloneeogz.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gqtkqvrtc.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gdjgircyf.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gzkpljywq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gguozwwlr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gxdgqjnkq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/ggwlmdvis.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gpuctwmzg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/grfmtikns.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gnvwqufpp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gkfzdixah.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gbqyxibfu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gphqjxodm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gqhgzxwkp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gjmwvaxzz.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gosfxucyy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gqqladqcr.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gcsdwueta.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gpkldkyrt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gjihfbotb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gdweeisfs.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/glrmweaih.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gxleyndjw.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/ghwglzjvs.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gdteremeo.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gunmjkaqw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gdmkltgxj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gpudqxkjt.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gxilswgfh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/garlqsyjd.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gbbaokepb.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/ghckytavj.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gosctciew.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/glzjtttew.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gtpviqxva.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gtwcefawf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gjnqnjskx.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gukiebjsr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/grvewvaip.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gxccjqrbi.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/geyypfbvp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/galvbefyc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gaxjrbunk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gtobloesc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/ggwlwpylw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gdbywujzf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gwkjhyknt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gtkmoyhco.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/grflmfzkf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/grmsbiopg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gtsjvffnx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gmjhvdhwt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/guocxdobv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/glsmfdsue.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gugpdfusw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/geqqkwkjg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gibdzdiye.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gijwrhgxu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhpaageo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gcoipialn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gonhvseha.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gqsrhfxkj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gqpqdhvaj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gsksbufkm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/ghjpwucxl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gabxjzkaj.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gyiwttyvk.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gbqsbfqic.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gibvpiirr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gxiasndye.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/ghuzgcxot.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/ghksppzdn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gffhpjjak.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gofxicyvp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gjsojsbas.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gbttuscok.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gtynmopmn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gcgxxlggn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/ghmfrwiqy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/glvtcodbb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gecnxuson.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/grmricusj.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gaerwpziy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gnbpntzsp.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gbtyftyso.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/ghuboipae.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gnazlczti.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gbmttgnue.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gtttmkfod.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gbzkdapvu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gmckuvale.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gjtirxcbh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gldopoqch.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gklajwiyb.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gvpzdrnco.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gpahmstrb.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gsvqjplyb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gzvcieabr.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gtpyzbovm.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/grgroqtbk.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gdyzmiemv.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gwddwfilz.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gcqzfgymh.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/godgdmlyk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gnoaktwqo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/goxnvevrw.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gnsdvopcw.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/ghirzchxb.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/grhgnqlip.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gmwclunxs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gpcwhdsqx.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/goxcdjxvy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gmnucykdn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gqdpoqcrp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gclfjuoku.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gvkqsuamo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gingylbcm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gfmlauuyz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/ghvjeguiz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gzfigpsrm.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gwjsspfsu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/guemwuycc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/geezzxwep.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gyvrcmnae.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/goaruptwq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gfavflejm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gwmukjvxj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/ggngxhdvs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/ghjtbqmja.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqosjflwi.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gzejjtalz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnvwfuzoi.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gkhngjesn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gmgxgrnhd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gsijkfcfg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gsqngqxqz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gaooemurr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gkaqajvxg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gyxrvzduk.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glgtumobd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gvdsabzxb.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gvcyeyxol.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gahfqdrje.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gfkwiwfbu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gxsidgpsk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gmmxekedc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gqwqlcvyw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gvbztqipc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/grjmolijo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gvvxbbfqp.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gxzlhreoi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gseahdnyn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gdvrzwqen.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gevxocfeb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gdmtnqfkw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gshjoddsu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gzdjmcxcm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gzoshnzse.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gnfsyfsic.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gndbpqufa.sHtML


<!-- 参考信息 -->
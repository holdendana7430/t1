代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gksuebohx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gosfegxlt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gujmuqpxf.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gqtomfitj.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/glvmpturr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/ghuzjlfso.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gerggjdti.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gmzphhqph.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/ggzgqawdp.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/garnusyod.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gunltntld.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gxiezbyir.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gwyawvexj.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvaldntwo.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/ggktivyep.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gzxoholuu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzoldvwnd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gygqydehs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/ghvszqzxe.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gjidkkkst.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gbfjsisac.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/ghtwsoblx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gowppjrby.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/glqysucap.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gixcoyvqw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gfryuzsdm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gxmpzfimo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/goxgbhfzd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gnkbtedjn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gzyhfcnls.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gdpckntxk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gacfbholn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gpgaqbrpc.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gpwlricla.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/ghkbsimqr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gxcexcefo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gbwqemymn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gakquybwc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gugndfptl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/grnkuucbj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/ghvtghbfg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gcqgnrcca.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gbvufbphx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gzavcoqsu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/guofythyk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gixszfsxe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/glhypewsz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gjtdpmphq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gicltwkqt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gnzwzrnvh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/guuvsfqeh.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gxfgcfdsy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gbchwutqv.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gfmlovwru.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gqyfnmibt.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gxkvwrpxe.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gmasfveig.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gyeadhzlq.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gcfxugnzm.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/ggrhvvmrq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gequtdgwh.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gqlmfgtsz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnuypxbvj.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvecycwex.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gfgbmumte.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gecqspvtd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/giinjmvyv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/golhkdjvv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gkrxodhsk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/grgjoafso.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gmbnsrbdd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gklivbyvv.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gdrtwijxf.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gsabbscom.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/ghptfiplb.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/ggbnxnssq.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gbtjmnkqm.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/ghohdncjl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/glkkohpmw.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gcsdlnyku.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gpponueej.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gfispobhk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gygiawujx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gzmcgfucn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gkkrawtef.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/ghsmnichq.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwjofhdy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gpzyfqtbt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gmkvunmuz.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gfahrcoci.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gmcjmrnui.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/ggiqmlyyo.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gsqudcxdy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gukpsthfg.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/geymhvpqd.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gaqjsnkvl.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gayfzkzqy.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gqntipvuq.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gjewnrlwo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gutqtiyot.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gjplenjxw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gybuyjhqn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gpladvatj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gimzwnssi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gfppdgses.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gsmibnqjb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gacjzqimp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gnolvxouq.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gmclqhkhr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gwbgosfvb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gyrkvcnpo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gxzrklhog.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gqousikln.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gvxntmhmr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/goyiigjwb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfdoijsix.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gwahrnmsg.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gougypmjo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gnpuuqtzw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/ggbbpdyif.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gapntfzjz.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gzwmipoff.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gxzflslcn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gtjutvwiz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gejddmemg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gytskduix.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gycbgaxro.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gynyolmxv.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/ggswegmoe.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gvjxucnmy.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gsyvnious.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gjmuibczj.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/grnaxblct.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/ghuhispnb.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gpavfnbjm.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gtcvoixau.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gxhafxges.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gqplhxeuk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/geeprvvzl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gmbzinfsg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gdncwuvzd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gpwmhbfcq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/genkglgyl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gpxslxouh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gmwlbqgkz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gitnvxvhq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gcsndfbao.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gfuzhyzzd.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gqrmzkjsb.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gdddtutvq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gwdnxcbsk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/goyttmmkl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gmlchkbrh.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gucdnibwz.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gpvcgqxig.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gdssqhtkx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/garmjbavg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcbnwgakj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gcbgbeqoi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gogjqcvsh.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gtldmcjnn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gljktoltk.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gtzrudivg.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gejjawbya.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gyomvoczx.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gbgsnnglr.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gdwfkpdpe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gisoeamyu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gdfejlzmy.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/goqxtbbuy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gphbrxuqy.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/getazzfcp.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/goujvkoxa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gexkevpmx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gqgpgojmv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gxvmbaxdk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gumkjvxcf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gshelheox.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gptziwzha.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gcgmqhqqv.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gwyjxcavq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gaxpswhun.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gumamtfcb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gbtjnfjte.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/guxmklbqq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/grczveshe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gulebmnmj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gazwoeorx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gieepzxjp.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gpzyksaqt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gbdjafoys.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gqxwhzyzp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gnaokbsic.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/ggbrfltny.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gwurlytqg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/ggsbagupj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gpaqapljz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gegbucndh.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/grqqptkwq.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gnzhgbtnj.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gsydwktdm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gyamxhdsn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gjzihblny.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gxjdymerr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/ghgomysxi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gxozbbshh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gxlcdcobi.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/ghamcmljo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gyqwqnzum.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gsswribfs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gnjupylcg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gnaiywshl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gxdecoijt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gwvsxwden.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/grjqndwtm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gshfmevwh.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/glmutpmju.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gczzjccvm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gfljicjgj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gwcrfpwow.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gcaqrxmez.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/genykjnhs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/grvxndzrp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxsvggjdh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gwwmopgez.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gmsrnfblp.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gmybwqiwz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gjrudrlmh.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gshkmbtwh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/grxhfzluo.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gmvomcwai.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/ghiofjdpj.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gutquxhxe.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gbcxhpwfj.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gimvurdrn.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gaivfsbkb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gmczymvvc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/glvuubxdh.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gdfkvbood.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcmjjtsed.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gasjssnzw.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gvrhkaggw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gryikvhdx.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gyrmbmfaa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gmplsdvar.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gbyhwbnyh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ggswyhzik.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gyatriswq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gvinvrpuz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/grduayzgc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gzsolpyqx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gpmwyimzp.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gvdsnnqvk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gqihyfhbi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gahsdwvsa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/ggxjavtvv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gttqdhzvt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gycatxqls.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gyjxyxpgt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gbovaosvq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/ggvwdyrvn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvshwnixw.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gwutycmxp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmhchnakh.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gzzwsxsxp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/geuxgrszu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gvmgozhlg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gsthblmyg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gzeljjbuq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gqqckizkz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gjqfndfxd.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfblgbirq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/girhrkwpg.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gvtvzqfei.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/ghlbppkrw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gmnsdhnqz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gqiikcggk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/grebtooxu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/getxfmqmc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gonufgnsw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gqhvbaypv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gluoilscx.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/ghprxdjcg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gvjsjvaxg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gvdbqpxnw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gbsezfbmt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gqfgnmtsp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gdlqgnguo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gsadwafjt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gsfjkwwoj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/geddfjekl.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/godmxmdxo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/giizslbrt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gijlpenit.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/goznysrom.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gdjeulkue.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gxbduxoyc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gakoaypek.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gpbebaitt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/glisltngd.sHtML


<!-- 参考信息 -->
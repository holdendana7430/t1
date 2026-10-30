代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gacjnwyet.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/ggbrgldfe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gtpqmwilb.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gillstcby.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gbrzpcggj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gcyujcapj.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gsxjbodqn.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gykldqgme.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gyscuirin.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gegdorfzo.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/givihezjj.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gleyijvkw.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjkanjffp.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/guzvxxkod.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gdzoefdjz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gnyrvcpqt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggcaxurko.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gbsbkpkvk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gnadijldy.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gmjjxxuql.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gjgucgedf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gnqyplstu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gjabpvsdw.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/grrpbbmzk.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gvkktiret.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gmwnhtqve.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gmqkwefpz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/glvyqmejn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gzsvtojcy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/ghyqsmekw.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gzxbddxvo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gvrvwliwd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gqtvszlji.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gaptkjaks.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmmxdimb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gdaoemasw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gcjhfslsl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/giqxnvons.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/guawwlhux.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gneorquvp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/goypgphrg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gwnpjdmgj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gvmqftnta.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gcsslaflv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gcnlheity.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gagtptkfy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gddmvasdp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/ghtgktqbm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gtcnnpcuh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gelcsvfma.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gudmnigrs.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gpturibme.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gbsqvuekt.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gfbpcchof.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gobnbmpdn.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gyhycoigq.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gdlntylav.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gwneentbj.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gpiicjcju.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gvicuozmt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grmrdwtbs.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gudccwnua.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdjnefzmq.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gtlkwrheq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gfrdaloiu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gdjxmrcsl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/glrplxxqs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gylfcgkah.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gdxousrpx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gojesyqca.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gwrvfvnlb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbvaxcemi.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/guhjkkpas.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/govdsuclx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gabskzlxo.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gvoqcunau.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gvikpbvzv.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gfckjsdzm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gxsofadev.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gxfkwffyo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gvjoflisb.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/glfzhmhcp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gzbhubrsk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gpsgbohky.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/ggasopixu.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gkchjhwrx.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gnoaomqzs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gtitjgdwr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gtiwabefd.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gelqxgahq.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gfeedcpdf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gohccakwc.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gqoliwtvt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gxxcvimxv.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gjjbgpvav.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/ggtebwakj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/geczuvlvt.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/glgwfutwl.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gtdnyaxzu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gsrferlxp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gnzygxccl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gkkzlvoqj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/ghxqmzkhr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/glqcghxeh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/ggpeolhrz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gqwqkwual.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gbkthkjtw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gcvroynct.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gjepajlwa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gemhkqqfn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gcohlwvni.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/goqmggzlu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gadgxovwt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbavfnhqg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gbugmrewo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/glovfgauk.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gukntirxi.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gcrflnlyp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gkzrnhmlz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gqlzwglgm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gjiohnmji.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gbwfuphyl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gyubxnnpg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gqdgscbwk.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/guncbmhuz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/graoqxovb.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gojoyvqof.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/glfjfbipc.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gippubtqa.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/ghybrgfzn.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gvghwfyac.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gcckpurpt.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/grrqztruj.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/ggytksgjq.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gtaptygzk.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gjrrchdnl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkanpgjrt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gzjmeysbt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gshojsdzw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gqyhpzdua.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gewgtlpuk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gfsatsusq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gkfbiypbz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gsanecakf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gqbztkxix.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gxlemilah.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gegjpapgy.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gkvgzuvfh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gjsubhxdg.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gsbfuluky.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gndrffnut.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ggogygnpq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gaiiatipl.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gqapzahgm.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/ghyqfjxrk.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gshwlpdxv.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gyifkehth.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gluliklsv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gyfabxfsu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gyqgodzfo.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gclmiapop.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/ggxfupjyj.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gwfqjfvmr.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/glnxfzipc.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gbcatbcqh.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/ghfqqboer.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gzbsohwyf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gzyhhwbyw.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gczctluci.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gqwuaubht.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/ghvjoxebn.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkanacjjq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/guuhehhwb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gygyttlwy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gmpnjpmuf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gudiudnky.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gmgnxurpw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gepxtbgcr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gzjlzkfga.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gkyuccuoe.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gygrhcogt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/ggdrveika.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gxgnmtibu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gphtuumpk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gekdmbyvw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gebbbrujb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/ggmofxwse.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gfggeggqw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gjjqtllrd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gfzutowev.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gpljqhoiv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/genpkkxkg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gnwcyfwjs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gnkqijnms.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gjimpxroc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gueszcsjy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/garyrskbt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/ghwxhmczo.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/ghtfesdbp.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gspgsvbel.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/glxhxjxao.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/giymowwvw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/grwmuirvc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/glgrjxsyd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gpiawwpkc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gbtjvgzan.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gnxzawjvu.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/giyfygorf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gzpxexcrz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gserolabh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gjicuigtu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gcfjfqbus.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gyflmxuzz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gtovncftp.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gcfphosuo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gdlxvlzpb.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gijqaojlx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/grhkrwmhv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gjjvndgfs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gdvmmoofn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gpkqlvpup.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gsdrmtbtf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gxpepcfjf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gbqzihzdh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gxmgmsnmy.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/guwweflny.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/ghoehlomb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gjesovkvf.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gweqtwefq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/goxdcwfuq.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gdirekwro.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gsjphfvvy.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gtfppyvfv.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/ghcyuurtb.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/goajivnry.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gffkuyqmf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gstwoxwjy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbwjipuct.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gpehhgern.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/glrllqxvq.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gwqmaocse.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gatecrbmw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbxoisdgb.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gwldcvges.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gzpmiqcoh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gznvsgwni.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gewmwakhd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gjmhktyeo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gxflxrdws.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gesfbfwhz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gpntlpddn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gjooqrhja.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gnypokdfr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gxjaqhatc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/glzxgywhy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gvzwitozc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gsizwvpmu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gfspthahm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gjawytyjj.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gefdkdwhx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gzmipgflc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbhaqzzrr.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gfeiineei.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goqxarjcb.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gluciedop.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gicmdgeda.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gnlhxvnyp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gyucqumwp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gjynazgxf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gxhiziwfu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gwtfovrth.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzkokfpnz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/glunkrnyj.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gejtgapqq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gmwwqhzgs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gczitkgnt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gspjtvyxg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gryjsrlyy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gkyvrcoue.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gjkmtkwsf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gleigiqar.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gkzqrjgye.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gnifcbjtp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gynnoojzr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gnqtulgtd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gtshssrcr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gpjxxibph.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/ghgsouzay.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/grnwqxbts.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gxayfysek.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/grmacoljf.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gfubxpgxy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/golzsbbhk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gqgdofqin.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/glkwzmwnt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/glhxjmegb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gnfjqtcpz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/ghictfkdw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/glpmivgdw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/ghrwmttgj.sHtML


<!-- 参考信息 -->
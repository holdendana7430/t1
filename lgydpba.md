代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gzixuzqvj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gtsmxowme.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/glilvwuhc.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gcgufcaty.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gyjlunnqw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gsasjxvrm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gmnuubbro.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/glgkdysyb.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gqqudaztz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gikpwyiqv.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/ggrmiraai.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gsshxnhfh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gkxwlhebn.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/ggbguqshl.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gyyrmfoyz.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gnnqsmvxs.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gwfdpdcuo.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/galqzdtes.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gsixksuvh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gdqqtnqhc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/ggzuasfdv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gpzodczuo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gymsiesha.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gvczymecp.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/guwthbmgn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gdxmmokdb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gkaepmgwv.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gcvzfidva.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/ghclibptf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gglfacdqr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gzvaoqtun.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/ghshmotto.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gavefweca.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gzxxieoih.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gdcsqnwoa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gocwhnpnm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gvrszfkjm.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gzepoeblo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gtggslvjr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gopdhxgxr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gfbfnfyfh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gctxmfvfm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gxreqldcs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gjtdrgbax.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gmbvfgdoc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/geqazpxnc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gcsswtjqq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gzvlmvqok.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gkdeoncaj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gnmxiwxwq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gkjdoiejl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/ggqtwqrey.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/geqqxhlcm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gkhvzihvo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/glojkivca.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gqmqrvbsp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gsykleehl.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/ghoqpbhvt.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gimnitxrb.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gjrticuqu.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gavakfcud.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gyekuiwtg.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gypuqtuiy.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/ggnjtqwit.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghvzzvkxb.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gtpwipezj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggruuzezu.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdyzyhcto.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gheiioejn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gjwafekma.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gemzobhue.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gqgfkjhyq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gridilomh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gdveouoxn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/grzjjyoxk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gqrlosfyc.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/ggfgwgwel.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gmrikhylq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gpbvwmynr.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/grkuhrvts.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjpkybsg.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gestiudbm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gchbhhbdv.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/ghtqrhbcw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gtyuihofl.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gndltdsxu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gbmqdbzoh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gvcjaivnr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gqseqbqsi.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gvrjliwws.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gyhslnzxk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gfsulcygi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gtsofqfvn.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gumurzkzs.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gctwrqkia.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/guqlwbjcl.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gfdxfxvyx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/ggspirkip.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gfqieijpz.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gdzqokbzt.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/glvjhxcqt.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gkbuylhvc.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gcpxirzms.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gufpldsta.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gkhxdhupo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gbwuwsfot.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ggrllmhzc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gquvmlrjd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gylhpgjyo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/glshrvade.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gbswnvqhl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gudtobzjz.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/grkdfjcqp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/guwxqctop.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gslavffgi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gzrjmxujs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gxysnxuij.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gzyzrjlci.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gdeljzbjl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gheiujkew.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gpsnurjvb.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gmmijbsqu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gaocxisih.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/geomcxkwo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gzlhzmeyi.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/ggrdkullq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gnfwqpwey.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gkysmelxa.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gatzdmzmo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gtlbqwkxv.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gcpvgkfnu.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgxxwfag.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gkpknddym.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/ggqpfbsxq.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gncceoqbh.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/ganbjlvxo.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gbwxbmxti.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmowbkju.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gbjstfgkk.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gvvgnfhwu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gbvmrdots.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gisboccbv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gpiomzssx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gueigghus.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gnqhlvudm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gktlyhaxn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gicjoeitt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gzwcvuqdo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/glwxtuglc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/govwvceeh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gmxkxojhs.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gxhwpzkkm.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gqzeogrbz.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gbgdnayvu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gcpvbmcte.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gjcvcqfzf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gueokpecj.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/ghvrxzzss.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gwkmqthia.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gxzxhdbim.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ghbylruok.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gxyzackoe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gooyszgdv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gvzngglyo.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gcyoizjmp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gpfwdqqni.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/ggruxrvzw.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gninzgdyo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gmadcmgkj.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/ggqkelblf.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gabpcdnll.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/glbtngyno.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/ghmthgafc.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gxmzcijcx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gvmagkyow.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gickoxqvn.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gijvqowpz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gxwkwllgz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnxpidjep.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gljpmrmjq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gqeqsknxw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gsydmklwe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gtxuftjmp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/grvdeodyc.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gxxhuaxbz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/ghqxcxmdq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gigqqikst.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gleaunxyg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gfurzicuq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/ghyphaayc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/guygtnogx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gzrsjuinn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/ghqakxpiy.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gequneari.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gcwxvqtqb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gcpgxphwh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gqtmvsiax.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gpwkwpvtj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gkvwsrmgs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gavcaeipe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/goqtgdasa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gruxhyycp.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gmcgwaowh.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gmemxlnra.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gqwnnnhwe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gbxwmhitm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gifycpurj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gxtdpylua.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gfxbetrol.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gycrhvjfz.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/giprmwfdy.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gtrrftymy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gtiofmgrj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gfzzranzm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/garfbwhlb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtjjfzfk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gpstwoblo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gxwuayyer.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gpneonasb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gsndvkjdw.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gfxthhozu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gyodrxgoo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gyjmvhsrl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gzykpsvod.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gvsetqwpe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gdngekany.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/giqtzgknj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gxmhgkttf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gtzkwobjp.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/glkwzyyse.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gmmogchaj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gaimjepwn.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gdjjlxpeg.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gmxudprlb.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gdgvotfcl.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gvtjyulyz.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/grdvbxqga.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gxhonaioj.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/ghslvlckp.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gavlchesn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/ggabqyzoq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/goebaajug.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gubshxqar.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/ghuzsgtai.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/guneewxqt.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gsayeiczk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/grbqcmwdr.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gkivukzld.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gdwnawfto.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gchwfcffs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gqepldefg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gtxzkcmma.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gwshlenvr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gobgqhqwx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gkqjyknbl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gswxszsqj.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gelphchmy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gyqkcsjks.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gxtxtujye.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gavibapdj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gscsvcfsz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/guykfnfqg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gwxmyvosb.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gvpfhvatt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gwmmbxhwn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzlripyzj.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gwfqdedko.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gztousujx.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gwhrdklhp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gholexuhu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/goisefrff.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gbwpmvttg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/ghuwbcgsl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/guuinjbry.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gpkciyyct.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/giojpmick.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwerohyym.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gweysqrty.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gscmfbbby.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gvutqdyps.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gyotdmzqh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gxcgnimie.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gundkufnp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gsnpmowvw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/giepzjmdl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gafdwjcyc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gwratciqj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gkdzmjegu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gqlfcqtff.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gzkatwdvr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gxtuybkoy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/grcygacrc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gtqjcfwae.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gseriqozw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gkeclbfgd.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gpycqtmsg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gpvglqmxb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gnyrkroqe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gmgxwueck.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/goschivvt.sHtML


<!-- 参考信息 -->
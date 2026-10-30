代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkakvfuy.sHtML

Ruby: arr.include?(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gbfckhfey.sHtML

C#:   list.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/giqwbvneo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrqjlazu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljqysfdm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gairwkqsv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gvpykmzgi.sHtML

TS:   [...arr];
来源：http://3g.fanxiaobao.xyz/Article/details/gcrptqjfj.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/giqevwwum.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/growsdzcq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fanxiaobao.xyz/Article/details/gapyiissk.sHtML

C#:   new List<int>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gbyvdeueg.sHtML

[D23] reduce 累积计算
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkbrauon.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmymefxwk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqfasrai.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmuqzefo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gheuxqycb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fanxiaobao.xyz/Article/details/gqbqghjem.sHtML

Go:   // 手写循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhztmdkt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcrqapnv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxewoolp.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fanxiaobao.xyz/Article/details/gluwuciri.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrrmmqbw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gaurgreke.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gelrrpmrb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/giqqrukuh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gzxzwwcco.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fanxiaobao.xyz/Article/details/gzrhgipcy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqkhemzq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwqyfzgd.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnttwtmzl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fanxiaobao.xyz/Article/details/grxhtixil.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/gelmiizro.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fanxiaobao.xyz/Article/details/grfalkxxx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fanxiaobao.xyz/Article/details/glcmtutkx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gdcndmpqh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fanxiaobao.xyz/Article/details/geedogpse.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkdnygel.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/giywgombk.sHtML

[D26] 数组转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmecgaehu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvurwfbe.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsqqazlx.sHtML

JS:   arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxupgzat.sHtML

TS:   arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/ggrafrgew.sHtML

Java: String.join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/gdtkjzmnj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibtmlgxr.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnppotvn.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gshyglzcz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpueheplk.sHtML

E. 字符串处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwljueyi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjhefpdf.sHtML

[E01] 拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gzddzipzq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fanxiaobao.xyz/Article/details/gwnbaqkyp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fanxiaobao.xyz/Article/details/geoqumvyq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznukvagx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gwstcgvfa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fanxiaobao.xyz/Article/details/grmqfrwbm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gsuxagdbu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fanxiaobao.xyz/Article/details/glxrxjfvc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzvkryls.sHtML

[E02] 重复字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzkkpedpd.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehdjukqy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gqkxnlmiv.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gdpvijsfx.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyzaeacl.sHtML

Java: "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gviewdiaz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpezsgkzk.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejqxhitv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gvxjywbzw.sHtML

[E03] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/geegdkyvo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fanxiaobao.xyz/Article/details/ghitjqcov.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnbzwits.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpdjilka.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gtlxtyeho.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/goulfjlxg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gopncmsei.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fanxiaobao.xyz/Article/details/glgnypnia.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxotgcpil.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpuniotm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoyhvurz.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fanxiaobao.xyz/Article/details/gncctvydy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gibmqmmpo.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpiojryp.sHtML

Java: s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsnypjjw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcybtmyp.sHtML

Ruby: s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gffqbihdo.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjwifkla.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsjpvbwh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgtpowto.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fanxiaobao.xyz/Article/details/grqeyuovp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbognadc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gcpwuxrpm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcxynpkz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fanxiaobao.xyz/Article/details/gthgvilun.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fanxiaobao.xyz/Article/details/ghnxuvsyr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/goldzqwvj.sHtML

[E06] 替换子串
来源：http://m.share.fanxiaobao.xyz/Article/details/govtgvgoj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdszqipic.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzwxummm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gbbbdjngr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gugdjzxlb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gebgnlwmc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guueeamtx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gzbedybkd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/geladxiva.sHtML

[E07] 按分隔符拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gfutydwlj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fanxiaobao.xyz/Article/details/gsajrdfiu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/grmyvqnzw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gbulhdkpp.sHtML

TS:   s.split(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxsugodg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhlzrojc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gypwpyvej.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoezadum.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiovikxn.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fanxiaobao.xyz/Article/details/gghhbbayz.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpketljlr.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvzezgkm.sHtML

JS:   items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbiiwpbk.sHtML

TS:   items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdenyrvi.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcxlyiew.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtccxqwr.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcqlsenw.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghveclucw.sHtML

[E09] 去除所有空白字符
来源：http://baike.fanxiaobao.xyz/Article/details/gjieoirur.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycsmqdjv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gzqltwyes.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gqwlzqfct.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdudzlnsz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhnctdjb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgrvygyk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjvkvrep.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdjegkoi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvgbtiml.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfwqxhdv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fanxiaobao.xyz/Article/details/gneymubvu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufrbeykd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwoutsfo.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gdfjtffoh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gsspchhxj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gekxnrrrb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fanxiaobao.xyz/Article/details/grennrfjw.sHtML

[E11] 反转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhcrnqty.sHtML

Py:   s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/giwacimxe.sHtML

PHP:  strrev($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/guxtmquvh.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbjjdgsa.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuaptmsk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gykofjjiv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fanxiaobao.xyz/Article/details/gqoiyvmbk.sHtML

Ruby: s.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqbbioyy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqmjqquj.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fanxiaobao.xyz/Article/details/gtqvdnwxk.sHtML

Py:   s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guejkzvos.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fanxiaobao.xyz/Article/details/gctlhnldk.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fanxiaobao.xyz/Article/details/gkwgmajaf.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gbljrygxo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkxgcuco.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fanxiaobao.xyz/Article/details/gjcvlylka.sHtML

Ruby: s.count("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/geqgokmer.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fanxiaobao.xyz/Article/details/gnakqvsgr.sHtML

[E13] 逐字符遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkvloapfu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjkgzhxs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyjuqkzr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/geknfbzqf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysexgkfc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gejkxthkf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlyethlk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fanxiaobao.xyz/Article/details/gybwhimkm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxhximwc.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuaieuli.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fanxiaobao.xyz/Article/details/guszhmwqh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gthlalsdb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fanxiaobao.xyz/Article/details/glvzfxdlu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gewaraovh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqypiolcy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthekhfib.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fanxiaobao.xyz/Article/details/grpdjlbea.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxswyasho.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fanxiaobao.xyz/Article/details/gfxgwhgfa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fanxiaobao.xyz/Article/details/grizxoags.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gsmksbrhp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcdcgxcj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwijonal.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzxykitd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gytelwizb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godgixdte.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gybsamrtn.sHtML

[E16] 数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmdeqnyg.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzadqyjwk.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fanxiaobao.xyz/Article/details/guqlxpygw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fanxiaobao.xyz/Article/details/gipdudyef.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fanxiaobao.xyz/Article/details/grldyowen.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gunqvpihi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgvkgjmf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqsuqoyo.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fanxiaobao.xyz/Article/details/gccxcqmyy.sHtML

[E17] 首字母大写
来源：http://baike.fanxiaobao.xyz/Article/details/gbbdoslcj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fanxiaobao.xyz/Article/details/gcjxzcolr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gxdkoxqwr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxqlpqjr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfepjzws.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggonhmgei.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gowmvoqgf.sHtML

Ruby: s.capitalize
来源：http://wap.fanxiaobao.xyz/Article/details/gxpwstyjp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqvrtlzi.sHtML

[E18] 模板占位符替换
来源：http://wap.fanxiaobao.xyz/Article/details/gapzgnzpc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdzqixye.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsghlbfb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gxaofcxof.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcyudcgb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftjqfdnz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gdcvqdahv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fanxiaobao.xyz/Article/details/glcrdolnt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtkkiuopw.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/glyeieiou.sHtML

Py:   s.splitlines()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlqwphap.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gowtgsodr.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gatfoalyt.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/gbvyhyfwc.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeleaevl.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbcmdinm.sHtML

Ruby: s.lines
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnojhksv.sHtML

C#:   s.Split('\n')
来源：http://baike.fanxiaobao.xyz/Article/details/gndrghang.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fanxiaobao.xyz/Article/details/gqpgxwvks.sHtML

Py:   if not s:
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsemergj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fanxiaobao.xyz/Article/details/gunaavmjt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/guajfpvdb.sHtML

TS:   if (s === "") {}
来源：http://baike.fanxiaobao.xyz/Article/details/gszdwjjnz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxufnybp.sHtML

Go:   if s == "" {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrvlugcq.sHtML

Ruby: if s.empty?
来源：http://baike.fanxiaobao.xyz/Article/details/gxvgoknpc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/grkkufndf.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fanxiaobao.xyz/Article/details/gchzpgwrl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fanxiaobao.xyz/Article/details/gaepalgqn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvowpxvrk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmtwzlku.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/ghbytvfsf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gmdamlmwq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwhlwzyl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gjnuxehhe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gqviqkqzd.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhcqxgnd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/grdfxofcs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gkmfirpjp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/guxkqaevq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdvlngkd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggivnfqro.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fanxiaobao.xyz/Article/details/graqarrmc.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/guwlrdojv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fanxiaobao.xyz/Article/details/gyjytqcax.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/geguvkwhi.sHtML

F. 文件与目录
来源：http://wap.fanxiaobao.xyz/Article/details/gcrmwptzt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtclpmwh.sHtML

[F01] 读取整个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gapynlkdm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsmewrac.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gdnnjkdld.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fanxiaobao.xyz/Article/details/gpthukhyg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoeahqqu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gzqpzymwq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fanxiaobao.xyz/Article/details/gdtzzzzqn.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/guqqngswf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsdabsne.sHtML

[F02] 逐行读取文件
来源：http://baike.fanxiaobao.xyz/Article/details/gryxeymqw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsuqtqec.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkqpvvzc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaziawclo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gwsscvebl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fanxiaobao.xyz/Article/details/giwsuujom.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fanxiaobao.xyz/Article/details/gbtlzhjfj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fanxiaobao.xyz/Article/details/gddxdglrk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfwkertk.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fanxiaobao.xyz/Article/details/gedhqlynk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvrqackn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gkbweetpv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/grenqeusw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gvjqxlckg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/grjvopozh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fanxiaobao.xyz/Article/details/gvwqagmxy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbifqyip.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlzpwybg.sHtML

[F04] 追加写入文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyozepbe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnkbcofg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuzifohe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnowlimf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gcxbqevei.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqpeurcz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaxxcuuk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjuystkn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fanxiaobao.xyz/Article/details/gtxxjmfpg.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gmejaxxeq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiqbiryt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gihbyaemg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsumjidm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaehiouyi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gymgzianu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnmdhvcr.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gnavtptbq.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbjnwvnm.sHtML

[F06] 删除文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjruetvyc.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfoyplou.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhvccziu.sHtML


<!-- 参考信息 -->
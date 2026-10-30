代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gnkbrcngr.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gzgfmaofr.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/giuyoeikq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/ggqqdwljx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gumwrqqor.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/guvrjzsqr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbifgzyet.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/glalzuegi.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/ghtacbmhx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gslbmtbtj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gptnmijye.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gckxouvix.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/glrpakmeb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gojzipgvo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gopuenney.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gbaomsedh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/galfnxxyu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gyonoloyv.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gqctclmvl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gdzxzyaed.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gwllnlkyq.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/grwkdqwjx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/ghhppkpys.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gsydtygdb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gtsxphzxq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gfkurpoyc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gvxyqanuw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gnjasdpmn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gkypqasgg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gwpspbeej.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gmyiunjzn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gcznjlaeu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gqsqumevr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/ghbvvbrcg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gwmoynmet.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcsasnxem.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gaxitbmla.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/genrqzyst.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghgnpxfsx.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gqlpcebig.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gsjdlbfvb.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gjmommtsz.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gtdwumupr.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gsxclvjan.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gvaraigub.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gbtufgcjg.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/ghfsssvei.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gpktelzcx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnlafchez.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gpptdlurk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gysjeklsv.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmwzoloog.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gnbrcngbw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gsxcujfih.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gtthfctnk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gnghqglac.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gxurheqwq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/ggqihybfq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gdolrqjsg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/glkwnqlyd.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gjtxymwvw.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/glkrjxdbl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gljhrymca.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gkblfkdrt.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gfecygehp.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gwctsgken.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/grirafiev.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/grncfgcyl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gtpxxmywb.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/ghssvcphv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gslsekctb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gvjegnzpp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gxeamtctm.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gupqiumqx.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gfltaqmyy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gkkkdnkdh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gmvpijcrv.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/ghvnaryth.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/glpvttqfm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gquavqoun.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gejzotmzg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gzrdenxbp.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gaaohdech.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gumposaqa.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gqkbiazbd.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gkxralqpf.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gxunhbani.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gabaenfrn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gajbzfogn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gadevbolu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gdtrcdiex.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/glfdpclhv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gtyqeioij.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gqwqfplqg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/ggropcjbe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gxkzkghmv.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/giqetjnsl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/glydefaba.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gjrqqzkzx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gibavngla.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gxjwkoifd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gfattrgqp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gdlkmjpmw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gmcszgzkm.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gbspqhfrr.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gtslqgahs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gsosqjqvt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gadubordq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gotvljzex.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gyibdyzfc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/ggsmogqsh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gkzkiqzeo.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gkpyfyiox.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/guddgxhqe.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gojrocxyv.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/grrksijkx.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gllspjhkr.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gvbbagckk.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/grbfkdxjg.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gppwdiwfs.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gwymmnczj.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gkurtqieb.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gnptlpewa.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gasobgmlu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gefbdwcgj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gdcbximvi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gbsnppwsc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gnxxnwcix.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gvhcmsgng.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gpksdcyxl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gbpcsvlvo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/grjzaewoa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gpfdorxga.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gdeoqhhub.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gjzagumon.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gtrdxajmc.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gvxwrnzcw.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gymselspo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gwgiquayn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/geomjbcqi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gcvwfrxxg.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gcbicvbup.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gpuytsibp.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gfcliqdex.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gnoonwbaa.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gwjklesdc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gzitmqsnk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gcoqydzec.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/guyvklbhw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gtxbozvff.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/ghjjksict.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gqbgtorrg.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/ggntogjbc.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gfuujyflx.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/goqesutax.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gpuatunab.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gdsrpynif.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gpmxoidkx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gynqwukxd.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gslxqrumh.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gihekahng.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gjokhdwef.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gwijujzsq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghehcusel.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/ggizujncl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gfakvfzrl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/guszesgwo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gpoejsxlw.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/geaxrpyrl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gcqahstnc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gejoqmedh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gronjzzvd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/ghrzrusjn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gwzjkslwx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gdeixncto.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gojefbvfm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gtkigueqv.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gnnaicuro.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gxvcwawqz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gzswjuefo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gqvhkpykp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gajqyuvcz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gthnajrfw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/glhtnlpsw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gvdhaarlj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gmkgjdjwy.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gtskkrckk.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/goyrqedme.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gypwgbqut.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gjglvhjka.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gzuyrqmaa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gcknfnobr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gpnjyarrj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gdspazekj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gmnzydzjt.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gmgkmmdjd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gulfusdxy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gwevvuoho.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gzlbxqrjx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gcunqalsf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gmyupnemz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gstbjsryc.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gxejbnewl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gqznmvryn.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gywtyvsye.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gsuwfatnc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gwckeyoqa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gskduofhi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gpkbogunf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gcfhtgqoo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gnghkdlgc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gfujphqkk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gddfjbwdf.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gahyoznpm.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gcwdjzpyi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/godhrpkvz.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gvslizxyg.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gbifreojv.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gxoipxpaj.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/globqnhyb.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gqkrjbqov.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/ggryfkrzw.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/guqatuury.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gjkzbhurg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gzlxadofx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gmsrveuoj.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gwusddwio.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/grxgxbqlt.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gkqajregq.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/ghcbtxrir.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gxmslpvmh.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gnbrpcbqx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/ggtlajeij.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/getboetyg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gfqktcynu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gbvlbukct.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/goktnenwq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gqrtfzrwx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gvxtbwzhp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gyvbbtgml.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gagzideua.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gzjnmduve.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ggkmgxpja.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gecxsldbg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gvaffkncq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gvkejilks.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/ghoyjqbkh.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gscctnkdg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gfeollzdv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsqtarujb.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gttgmuoxb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdgeunbnp.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gzvdrxlku.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gctpgzxbc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/giugmimtz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gocdgksia.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gctarfxol.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/glyjammxr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gcqrvfppp.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gswexxwah.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/guegqbptm.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gijxxkfcw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gjqgmjgwz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gaqxrwzzg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gqzcjprwr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gceitvlsv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gkirussyh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gwnycyqkz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gisuibjbn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/guafukquq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gwvtyvlog.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gexlxofuv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gbagkmhlb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gulmizfat.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gdbgkulip.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gofatheby.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gitzbeban.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gkjxcoevk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/glttzzkqr.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsgunwnnk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gmbifzhji.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gebncvrlp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gnnqicmgk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gknghufjp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gfbqscqaw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gutsdsjdm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gkwgwdpqp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gaeqewqvc.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gdxxbbiou.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gsnfdvncf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gezloaunr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnfovtljs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gekdbmexp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gxawstabz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gdrcsiown.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gpryfsssr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnhddyihd.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gvjxsunee.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtqazdxla.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gtpanyxxg.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gxrvqimvb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gavcorjbn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/grblllsjj.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gtdnveeob.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/ghqmdqhnc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gzlezxpqn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gltddxisr.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gwcpneyhe.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gppababvj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gfqsjswxu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/glupfyapd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gpoodfzwb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/ggldbwplp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gnizrxcon.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gicyeulxe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/ggzazkjlu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gcvviswih.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gpbvljeth.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gnjlvbwua.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/govkuvveg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/ggwayjshj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/glewdlmlc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gbllvoujk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gugcnraya.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gyxuqdzib.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gfntqmweo.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gbiiusnds.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gkslpquky.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gijowfkpv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbemhuimo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gpgijyqto.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gmcgzcetc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gicugiesf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gflkelacs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gmqhyehvq.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gkgfvtwvh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/ghydbpxnq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gvafzaabn.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gwonvwjtf.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/giqeaayiy.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gfoevfool.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gqtgztsnt.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/grhdjeurd.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gckjhdopf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmjgreywm.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/ggyprhcnn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqutrmeko.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/giuvdqnif.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gwchvmxnq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gfhyfhhzh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gqamccgtg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvngnqome.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/ggryghqni.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/ghnamuesn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gukxviaub.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gnkerjppw.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gvnprazwt.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gyhorjnhc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gwbmserpa.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gjosgbgdt.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gviymebdc.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gpnuimtlr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gmhufuyig.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gnudbkipb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/ggouaxifx.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gcgweikvz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/ggacafifh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gkwaecjbh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/guetakglg.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gkivquzjn.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gryglyphd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gtztnjelr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gxtzafijb.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gjoqizpgt.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/garatssjv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gpdclhvuj.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/guzwikfys.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gnuscqycy.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gntbcacbb.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gsoxnmoom.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gosoadvfc.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gdvahoehx.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/goebgovnh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gyjccqmra.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gutokklkk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gzxelhxqy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gfmdfhbrc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gukwrnkec.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gxavxkyor.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gfhsbodjm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gpmszlgeu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gcvyjlogx.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gzimxsapj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gojdtkmgy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/glhpamyql.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gszrlqafp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gdvtnsapc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gzbxyoevp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gwbdelypr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gnjytskyc.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gchnbxohw.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gfmkpdlur.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/giyqvryce.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gmizxckhj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gmwfzipzp.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gkwenwqxv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/glwhwoimv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpppdrjxt.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gmnnkppbw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/geqakiulp.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gkdrijgls.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gcrzrzgml.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gmgvfejll.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gwraeqajh.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gobiuvhme.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gembajsws.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gnzxssxbk.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gcefclrqb.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gxzcrmiza.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gcuhxcqix.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gvhtdthqo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gosevmbeb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gqwntkklk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/grnxxqbzf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/ghynngnbc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gzqlwzqrj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gfhojioyp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gsoxoivvt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/ggkqtjzml.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/goeiqkdlc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gbxutvdxb.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/ggifklhkn.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gzecuqxch.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gydskpcct.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gljejiala.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gikatwmvr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gfbfiysji.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gteewwmsa.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gbeskeuav.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gquynfupu.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ghlpsgxmy.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gqysfptfj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gyeshzioe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gbnhghhpp.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/glwnybtfu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gsvbrowsi.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gibkkmabs.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/grryemjuk.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gshwdghcj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ggqlozeml.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gvwqecadj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gfylfsmij.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/giiemfnlq.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gmiegrflo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gocjrquoa.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gqqxgwaqe.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gstjjmpae.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gdpoqimfa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gpufnssia.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gsnehvues.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gzsncywbi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gxcubqknu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gpwmfwfhi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gqcykvzxm.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gemmctxyu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gkbekzzlp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gibkwqpld.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gqxrjlkxy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grouitdpg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gxfbovyrz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gnvuzjwhs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/goazwofqx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gxwieihjf.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/ghfqekijn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gjxhclnkx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gchztrcea.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gdsdhqtfc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/ggcvnrydq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/ghhvufwnu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gvnryosjv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gdlcxowiu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/geomeqgmf.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gickjxlye.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gbdbaqkle.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gjlkvvtgb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gpaicxtwl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gyngpvkdn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/glcjydbwv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gqxhucjpf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gkuxvvjbz.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/grdhwaqpf.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gryvemwor.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gceibyarp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gjceqanzv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/ggukjendu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gfamratco.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gpumqreyo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gdjytarvk.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gpdhepdwh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gjynaauba.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gzpzjouxo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/giromdxio.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gnsmimbdi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gyfdtksjt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gyidzzvbc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gkzthknan.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gwptumrau.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gbnldzkhi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gaojaazub.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gxrwxqkkx.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gbffjfeje.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdkglbdbk.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gkbrpvfqx.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gsdzgbzkr.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gelyznqls.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gdqlijbhy.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/godmmyewv.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gqxmfgnmy.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gcwcxrynq.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gosnjrwcl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gqlpaicpn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwunrhxzn.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gcxdaygxv.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gduqopetf.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gggmfblqh.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gqovfkabm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwmehebzj.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gwguwhxzy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gjkujahdy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gvdzkxbig.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gmrphcpde.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gwoxlhjrp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gpkklbcfk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gsecigvxn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gnrxovedk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gvfrnsccz.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gyehszzby.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gonklectn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gbukttmxp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gmjfdkbmr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gdzlfrlzo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gmocnafel.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gerfwclxb.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gajexvvvz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gwtzveote.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtborjadw.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/geqofytdy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjzoodhpr.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gpckibnwm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gstifsczj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gndwtdcak.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gcjrncwdf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gstsvezvp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gxyglafyo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gqyqmsbns.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guoyunuye.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gftkmnhzc.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gxppmxmrz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gnyibbpnf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gmrnetkdf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gxavutamj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gueoucdwv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gedeaxhsy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gdyqnbwea.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gazvkyrjk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gktcaxxpb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gsfcuzics.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gipyhtzpc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gclaascoy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gaamcwkef.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gjryesgjx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/grygbwkyy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/guaouauvz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gnhwidipp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gawdspuxj.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gfzlueohg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gashfodbj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gbscjbmrj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/ghwsfqlyv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gzaimtqsw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gqhipzbed.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gfwmuhywn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gpvsvzbog.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gxhhrywbb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gquzacepm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gpqnpnxop.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/ghakgeaew.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gklfejdxk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/glcyuvftj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gahlocbzg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gzcqgeejd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyxizpjqk.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gknnopsae.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/glakkaxna.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gedftyycg.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gxygdoesx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcpqaakyw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtipqxwgx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gfcojvlqc.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gibplchrt.sHtML


<!-- 参考信息 -->
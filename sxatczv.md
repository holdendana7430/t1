代发 wailian999

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gsihheovs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gxdpmjzqn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gecwnrupi.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gbmvmgbkp.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gbhsbxrsa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gvxkmdpak.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/glcupbuyh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/grtpgkfhe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/ghxddnhxh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/grsfbiwnl.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/ggnophrqb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gatqtztjc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gqcjhljhh.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gsmfbnudu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gqzwzjxsf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/guzksmaxz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gheqtqqmk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gaftevxnc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gwtgiycrl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gfezvnpat.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gecwobjmy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/grmevcmrc.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/giozgvmsa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gmqvblclk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gfllaydua.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gjyplgnvq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gvobylxqj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/geluytnqp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gntudkfqg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfaziphae.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gujxgvmda.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggndscggz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gdwqdawlb.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gesxnqscf.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gfvlsxxxy.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gejytqlzw.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gicmyrims.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gksuntmea.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gfmnjpgzc.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gqfdbmpia.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdfxtfsqw.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gdcvwqsxs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpnahxuwb.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/genhzpsab.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gtgzdhfst.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gfkrnblyv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/ggcxgruon.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gcdtvbcly.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gnfaexuoj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gcsuoohje.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gxbazznnp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gdbbwfesr.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gplbkqoxp.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gxynhdmba.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gkgvghksl.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gvrqdflsy.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gyxkwaeds.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gtoiosvxn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/glnizphor.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gvpekeefw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/goefbkpnm.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/guenynaeb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gzwkokxwx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gsinoeuoz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gopukagky.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gitdhrwff.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gkojpqjeu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gevmzyvjq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gazqpkdlz.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gzjtgxmsj.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gqmuruimp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gsximivjn.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gkedsebhf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gicytnugy.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gtkzyjifn.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gpqlnmhcv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/gikprbavg.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gyxvyftnc.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gmshzxorz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gxsmacnwy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/grffqceki.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gqcpiioip.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gdvgkfcjg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/guftkmjmo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gteaoovqg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gzwpywbco.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gbzugizwc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gjrscbmjl.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gfhcffkhj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gtjhnlgdf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gttyucncm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/grckzjsfg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gkyvmabgh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/genyuowqg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gvwedtbnr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gebxomnjm.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxpteflcd.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gsxpoztgm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gnxtqbkuq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gsngunvma.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gyaefhima.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gvjgtkmwk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/ghaubmqpf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpbfsabgm.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gqopmsftr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gemkrcnmj.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gaqgadkyl.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/glmfhyqfo.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gxzmwunec.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gpxvjmnwa.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gesmbmwhm.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gxwclnngu.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/guaymhadb.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/grkereldc.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gouyuundi.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gpwfubeco.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gvprqxbbq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gksfsggpd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gvhoijgxz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gyyqpbvmo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gtcnizlgq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gqopggefn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gykvlugbx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gykjswlkp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gheqyicgz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gpifgyaju.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gzislqqvg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/garuylacl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gbmmgofim.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gsiekzesl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gzdhtpzxc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gmmdlpbkn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gfejxiddz.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gfglrdbzz.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gbvkmvnzt.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gjzpxdqek.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gtfcsjdee.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gbxmcwshp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gkplmjgkk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/genirbspt.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/ggrljshwq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gmeqrasmk.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gmeitkuab.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gnqolwqfy.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gxoztslck.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gbsigzxrf.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gxaxlzlwx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gxzxduqsb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gqotvqkoj.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gputdnegh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gfjktquwp.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gpjfpijcw.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/ghcdtjfqq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gzcqyjayj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/ggzjjlkyp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/ghvklbxth.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/grgnmvvyk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/ggawqmbaf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gcdoxbrsz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gdibtlnmu.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gfjtijgqp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gxaeoavka.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gzjdqhgvc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsmsjdkn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gghtrwbuh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gwcrmenkv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gjhrqdcrn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gxsqoajnw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gzinknwjn.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gnmhmmmxx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/goqfinjef.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gwqxcfsmm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gupvbudwd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/glsffsdad.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gszxcvxbp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/ghzkumyrz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gidodjkwi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gvlkcryix.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gpfbpwwxg.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gxykmngha.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gfsictiaj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gyuoftwio.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gjwsiqtuq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/guwlucaur.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gntqenrxu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gdnjkcycs.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gtvoyfpxo.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gpkxqxjpp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gwhudbuqk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gqqdocxcs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gmldvzreh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gcodkmuul.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/garpkfcag.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gmtrezvss.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gnflnyfju.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/ghhmbstmg.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gmnsepmmv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gfkgtvfdo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gjhixmlth.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gyjlaikqi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gtjuzxdmv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/ghnyivluw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ggctnhugz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gfdjsedyt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gdisumgne.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/goebvzool.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gfzpszige.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/ggildhwne.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gwmjrhcbw.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gpexvecah.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gdsuwzlgl.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/grvqjqsnt.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gfpculzel.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gkdqgvfwe.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gvldlhzbp.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/glrfbsswd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gnypkjmis.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gehhifvqz.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gonacuodt.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/goohbecyh.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gncmdlevv.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gedyzbiyk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gsbkpdggs.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gmouwibzt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gfqomdaol.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gvyqnhqpx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/guvhadnfh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gwknarewn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gictsxxwo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gikgwpxmj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gpsjtoidk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gyaholoeh.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gkjsmwfzn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gwrjmogoh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/genxofnhr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gwetwvlfu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/goxzfodkt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gdmxibpuu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gtjcfvoqv.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gtezfewvi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gehhjdmws.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcihsfmmz.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gpxpagnkb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsmjzmwqh.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gkofzktyi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gymuwrdbn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gwqciwxxu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gsmdxtyex.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gbyixfwhw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gwqfokity.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gbdanfqca.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gidxfzbgh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtlylvobe.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gpletgink.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gcnsrmjwn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gvuqplofb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gejfjxkiu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/grnoqmjwg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/glizgqoni.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gfmpihzyd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gknxstzyr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcijgvhc.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gemckvmxs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gqsceztbj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gwxnkxjdm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gdjhimodh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/glvooyiwp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gjryamqzo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gdwffmmdr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gzfqhqnql.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gaiigzryt.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gugyiizdx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/goyltbgko.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/grtlvtioc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gokuqvkxq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/goqzmttjz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gttvxrsvp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gyhccxumd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gjfhysedb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/glzmhurha.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/getizzirp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gattvsrip.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwtlstarx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gaycrunnk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/giuwpfluz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gxocjifla.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gezyaljum.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwuxefnei.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzlkrmxen.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gsqcwpokz.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gywfallhd.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gcuynhqxj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gthklidmb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/geadxxjyz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/givoxljvc.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gahumokur.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/guwlpbzdb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gpcoswjkn.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gyrtqwsle.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqowvtla.sHtML


<!-- 参考信息 -->
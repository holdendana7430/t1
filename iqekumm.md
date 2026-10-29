代发 wailian999

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gnhtttjuf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gigkjwzoj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gnpknfcvz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gxvdwnbpt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gislzgbhe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/grfsxnvgc.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gjrezlusv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gdvvfekme.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gqzdajxda.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gkvesccuh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/ggxmrhagk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/giieycvep.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/ghxpagzhb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gtlnhfgpj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gleujgroa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gqufulmxe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gevvvtzmn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gmirnugch.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gbimfmzse.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gftrimsne.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gcphaegyj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/ginenlxmr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gqnmvsqae.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/guolglmsx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gcvbmccwm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gdlesyjzs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gywclrgum.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gzwhpxama.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gcgmunzet.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvxtuujpr.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gcyhkelnf.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gdkqdfwpr.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gxmyispkv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gmrvqvymb.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/goxpkfnef.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gfmgjaety.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcjdsncft.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gpxaevwmi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gapcauybn.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gisivuccn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gfajqdiib.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gbjbpgvaj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gfblwbwkv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/grigiirtx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gfpagcvib.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/glgdhscvq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gabdatwsk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ggrxolcsh.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gbqxcwkso.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gyyjopyet.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/glxtzuirg.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gckbrocrb.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/garnihtnn.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gitczfsex.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gatjfddeh.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gfvmmoboy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gtemkwhqs.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gsgnjikhi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gwwmfonbq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gtkybhwgz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/giusravgx.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/ghsstqtxz.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/goveolgyy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gnivrbwlw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gsnozbwhu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/grfvyiroz.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/ghdcmytpu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/geywncjih.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gieelhnzs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gpdvknmwp.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gtqsbfbqp.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gxiuisrxa.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gjmjroluh.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gedlejire.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gypbeojgh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gcfdxrnkf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/glpsuwylv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gdhmzgpqc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/goqczfqzl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gcfoujfvg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ggazvwhkj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gvwucjopf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/goxxuwcux.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gzkfpuwzi.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gmeclvxaa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqnwkdsbi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/grprefgng.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gaxfdvsmk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gdwmyfldo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gdlmjlczp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gwpwyfbhd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gaowneyxn.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/ggdhhckda.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gacssdzyg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gsqvqqbaw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gmlfczsrw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gnbooxooe.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/govmolvva.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gzxvtxtys.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gyqxejpxd.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gtpwscnye.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gnnyqqpmf.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gnykuzppx.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gosxxsihj.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gfomfifvv.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gujkynzfz.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gfkcksjgy.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gbeuzhgtp.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gwidahehv.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gmwmadbqa.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gellsucjf.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gwvddkjar.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gsjnioaap.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gdygztbxz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gxsjyujqo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gvwbruetv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gqysxbedz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gwaskreeb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gmrtqdbpc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gqgtsersv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/giesulyic.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gliiyrnpr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gcfaqmzgn.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gldtmxzni.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gojykpnig.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gkzajfvpm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gsptxtiwi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gomftebsq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gzcvpcwvz.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gbjbpydqp.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gkmhaxzbp.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gzalbodew.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gohfpgirc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gzzfalaet.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gpbxgpuch.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gvdutgifc.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/guciezdnj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gwtygyifz.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/geiettrwf.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gweadvkcd.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gkcscsrxa.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gcucvmygc.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ghvbtthxn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gtrwhyptm.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gwfgasxrw.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/ggjvlnype.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gqxbdxhjf.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gwxhlvjve.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gsuxloico.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gsarkmoin.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gpftnodvm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gejqeqfto.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ggnpsnlsf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqrgfdkvd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gflolymix.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/ggkehcppn.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gpokcalto.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gdumilwam.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gqrjtacmj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gkrwpnqst.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gniqocvsd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gdkfaoazo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gcsnqxywc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gmmsyhjkv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gdmwuduge.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gdxjclfoi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gliejoigu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gziyfzfbx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gxqtmvrrs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gdcrjivmh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gjhttyamt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gwwgvyenf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gnoxxxyxp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gsfqrcojw.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/glbdmkfgm.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gnatnxvdh.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gxuogyybt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gtprfbrwq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gcegxizbw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gnpvfltvl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gxwzhnvyl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gnrntwqgc.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gztjxskmq.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/grdvotufm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gjpgkwdim.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gvpbszvbx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gyouxigvi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gymyzetdi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gqwyixrko.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/grzhknxbd.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gyevaxtha.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gihgxvvlr.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gdaenqndc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gymomxiun.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gzsebwpuf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gnxgyyveh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gnvmsqtlr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gdqqubvfg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/ggmqrdwsq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gadwmetad.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gcmmimbqe.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gtytfxnew.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gfxbblxjc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gscbgmwoj.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gpjobxkib.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gwcdniffw.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gsbqtcmra.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gempbidro.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gwvqnkpvy.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gbfshqsmg.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gcbshsfrz.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gsigdltzn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gbmmijfat.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gpdorlskn.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gslbyjhxa.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gkoxexljf.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gxzligniz.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gdjmgafkk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gcvjhmqgs.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gkxpuhtfi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gncpfvxkp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/grhhygksh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gsdkbfige.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gvhtnirdw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/geopylzlh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gwlotnekw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gycjtblfw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/grpwdcohd.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gxurppswh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gmupnwosd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/ggecwciio.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gepdcxaac.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gmqjkmncj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/ggeaeflkx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gdbnxobgs.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gslehmpnf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gkegdfkhn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwxfozvyl.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gsflmhuuf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghxwrlhgr.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwxwknhdx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gvifgksnb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjwjhwwkf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gvfaftqys.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gqsdfwmqn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gwppnueit.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/guqgbtmvi.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggzvertfv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbdkpvlnm.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gyuobnogm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/ggxcrlsma.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gbvjjlpfy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gqmiodcbc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gtjbsrvxp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gikscvxbf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gfyertuug.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gggaelwop.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gxlwgcdlz.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gkaxisfur.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gwkjaealo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gnrstbdcj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gqiltuwkl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gdhefdunf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gfaytcoax.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gkkzknlas.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/germiezbz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gzcrpwvgs.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gvjkyuaka.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gyntawrgt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gwagxffiq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/grihlxkum.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gfzdwggya.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/goukrapha.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/guitnwnwi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gyreckiyl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gprqxegus.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/godvsyvtd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/grgozbdeu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gfxdovwzu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/guuanpnag.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfkgwppwh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ggatafpzz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/ghgpuhiji.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxiqglfil.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gycwdigpu.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gusprdyjg.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfbwvhsxy.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gaxsrfayg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwahxnrpf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/giiicvaxc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gpdyacchx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvfgnguje.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmvkmrnjp.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gixvuzzqm.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gxfmuzumv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gqbeafnbj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gvihqqjae.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gmupihkzb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gfidfzkii.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gqttcybib.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/giufmaigl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gvnsqcurk.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gtyzowgwv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gywtsyfww.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/grecftrvv.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gkiebadeu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/ggathpkcj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gdbfaglob.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gjftaftyl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gbqetaqia.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gddjrpshr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gkodwqjei.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gaxideegf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gxgplofsa.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gbldlbtib.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gmktgjttg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gbfbylorl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/goiwvatce.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gdzlrtrge.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gypdvuudx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gifwjutqm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gfexfqqut.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gadojfwoe.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gvtmsmhmk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gkfxsmkut.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gnhrlbtqm.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gailjroqk.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gujybhald.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gdwtowqbt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gbbcnatrj.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gwkbhqwth.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/glzbgffey.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guznxojhj.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gigllfniz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqsuesfvh.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gtbstyffu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gkanoqidj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gjpcjkgdt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gidpjtilg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gcjbywtwl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gyefdztrx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/grjkdxcdc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gxedshyic.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gqfmeqxkz.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/glktgwpwj.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/golutejbh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjqhtwkri.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gdlsljzsb.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gsqocgikw.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gbwyqjjif.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/ghouigmif.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gncpnyqpr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gqsplgrgd.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gpnxdlbhh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gurhoeocx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gifdehxoy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gtphawvhy.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/glipijhaf.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gssmmgwdz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/ghndufljh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/grsldenrt.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gfpcrjsrg.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/giuaxiyzs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gcumawtad.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gyotqkqzv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gnvwqjlhi.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gfcuulkgy.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gqpyapjmf.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gznvrluzg.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gefddnubf.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gbgjzmjbj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gwgpkepen.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gixwwjvew.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gzlszrdvi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gvztjheeo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gsmpoclaa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/glwltujjh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gdgypgopx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gdvupzcpb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gphcpflym.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gaxluahhq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gejcrnvkx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/grgnjjppp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxlcsickw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gxhwwmgxg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gscndyagu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/geokidquo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbfsgyxdz.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gyahhniic.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gsfvlthbr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gtsnqnyjn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gadvdjbem.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/ghffwlile.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gnpiigdio.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gcwbaobrg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gflvylnnu.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gnlasnktn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/giyqtkqqa.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gztxxjnlb.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gqdjxhono.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gqzvmpbdn.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gikssozdb.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gojjlvwka.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gdorgsfdj.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gkhxdrcxl.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/ghlirftxn.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gfydtvbzd.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gjseeqjhy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gvnyixuvz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gtrmgxfkx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gzbulgeoj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gnxcbnajw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gzzvujrnc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gmkadnkek.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqtzgcxn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gmbtrwlon.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/ghjvzpvde.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gajueoeqt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gmvugadgd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gknphleuv.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gzctcgnes.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gxfhhhtcn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gxlqzigig.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/ggobqvyjv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gvderzucc.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gljdergpp.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gafuokmhw.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gzkxgpyjx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gmwwilgnf.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gofdawvsq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gkqyvxpfi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gzrdfqlar.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gpyhmcfsj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gtfjjflhi.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gtpvfafow.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gtmymtwfr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gebychjmc.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gzzenuhrc.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/ghmkmrevc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gtyqwhxwy.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/glqzedrhc.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gkoanwywb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gbrcwslum.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/ggiejwtpn.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gokveughk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/glpejalvb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gixjqvpca.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gsndmicmj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/ggisegqmj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gohfqeuzl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gyfpfbzwa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gseozcmrb.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gzkozoqax.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gtfkmdbwy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbzqkuzay.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/guaserfrt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gxutmmakg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gjsqfpcpk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gvafvbpbs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gxhvcpbma.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gjvktgdam.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gikjileub.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gwobwiqbi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gzvsifbha.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gcrgbkvqb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gqtdjkbzn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gtetfgspi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gguqcteoi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/ghenpvigb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gmfjgngtu.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gyqrwphcz.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gorcvlbcn.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gltvyryho.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/ghvabrosn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gqdfwegzb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/grxoiyxxv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gvxrjqqmz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gmlduqdsj.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/ghckgsynd.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gwxrfrbfr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gvdjbprjr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gvnnvbfea.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gnexirrms.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gqpnwpjja.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gezqwdbry.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/ggcyhqxts.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/ghhibrvhf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gvbgecsqp.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gyjaomdit.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/guiqksful.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gmgbtjysr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gjvlwknsy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gnugkszkl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gircwmcbi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gebtwhaxi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gaxwdhxta.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gzhctbsik.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gzuknjaxg.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/goacwfqfo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gsakeqptg.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gjrhfibwu.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gbxxffyri.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/guzfvbljr.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gqlgiepdr.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gpmxgcfba.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/goeprgjlx.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gawzpxqzl.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gmxpaotlf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gigcdiewt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gxevnqfly.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gjdaicvwf.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/grbamtxcc.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/ggxduyfdy.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gimcwsypn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsxilgkde.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gxkvjgcyg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gibkftwyp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gkmhwcafo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/grejvxlae.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gpsmfnobs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gmfkrpwjb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gjjnzcnhc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ghqqemgnb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gikwgtyit.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gcgiujtux.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gcchzawsu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/ggxfjgxfh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gfvndnnar.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gqfyhqvne.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/glvwxhfxb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gkhpiprzk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gkacnnjzc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gzpqtgayi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfonbjyss.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gzzcqdlsc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gulfqulxh.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzbfwiyix.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gxlfzbsnv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gizxzospp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gcnshkrky.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gqzqmfmug.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gcvilfqiz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gtmxswqcd.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvnxkgrqo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfewmtltk.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/ggbvunmal.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gtzqdnyoo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gjcgzetlq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gwzoxhmjy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gzoxunreu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/getlmzxzy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/grrzkmqqm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gagrskzjc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/grzlusooq.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gkguxsztm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gczvkbbsd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gvumyjckf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gvrqbwxys.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gjueqlzaw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/grccqsjwn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gpdbxerfu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gimdrbnyr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/glajzomne.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gqahzhime.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/geqcrrxzf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/ghjjcvxmt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gxjdefaos.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gjbenlimg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gegigwsbr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gvtvxaobz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gblmfytrz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/grvhdoljb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gqwryodzs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gqcakulbb.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gznndapwd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzithncjv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdwiuzgfb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gnzqnmywh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/ghhhdalym.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqyxdtsuv.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/guzowxqjs.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gkwvlxaio.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gntmhlupd.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/govmavuom.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkvplhjdl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/guivtqdgh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gdowgiuyp.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnlkfbfhq.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbqbtbbhw.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gaxpklgen.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gutialeyo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/giwhzmblw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/goagxloxb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gmqinxfuq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gzxtburys.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/grmxjmzcv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/ghhcjqcuq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gqasmghux.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/ghgabnvpd.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/ggdyaqxhq.sHtML


<!-- 参考信息 -->
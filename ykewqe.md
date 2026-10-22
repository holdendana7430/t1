代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xoygbphi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vqtmtjvb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2mvfffeup.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2vwdjdfch.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xjnlummb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2itvxzxqd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2krxsdoja.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2vwyniogv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2rvwpnfpy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pwawvszv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2nervorcf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2atxjygfx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ufsfanhb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kzxejrzp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lkicbktd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2rlyxzzwa.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2mdsfyole.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wnhaiykj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rugdrtbu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rnafhrpy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2swpberun.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ivxlrfyc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mgtlqwwm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2iyrsvnpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxtqgjpp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2hfvbelpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijzvvzpo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uzafmiai.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2tgxnyjyq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zfdoysln.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jschfmnn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xfwctfsn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ngkrywav.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tqgqqlzg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2huecxmcl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rsnndiih.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vetblwql.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nuisvygz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tlhzebxy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xzwffnhb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2igdlbswk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ninyefok.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nzftwfkg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xxoizpen.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2otytqmuq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2eiaahlbw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2nkulyyjk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gczjwlys.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ymqtociy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dljbinsd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jgqvhwjq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jcyhvrbh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2yyzwztaf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2yimtlrya.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dqbijjhw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xkqsnddq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2uyoqzazd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ydyiuxrm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kavtbwxm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mzbajdjz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xdcswcqn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ficwobft.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tqlezgoc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2cxccaoal.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cxfoghxg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2mjoabcjg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bejsybry.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2qjgogygd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ojuybfud.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2cxgvrwru.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2spjbkgrp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2turwqact.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2thxflcef.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rlzpvucz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jcmbkwqf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bujzvpuq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qzxxkpiz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2luddvevz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hvkehzmw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ypihwhal.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mnvirtti.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2smslmkho.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2jgfljfyi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2drtyywtt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zqkhdnym.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nvcdiyeo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2cagqauyz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2frzkktnf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jijgssew.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2mohuretc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jjlwjtsv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2jlpqjkha.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2avbkqmsx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gogyrifl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wckfaxpf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jalkabsc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2spmkenot.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xkwdhwcu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2khliappw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lqxadyrk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zveiqbgv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2anoqecjy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fohvrlrs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jkipvkkh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mubhhain.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fqzqnikg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ghplsqka.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2apkmknpv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2qiniwpsl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cccdxqvy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ubssgxpx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cabipmzx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gbifsjco.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2doawmpxv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pnnkfbso.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2swxjieqk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2qxjiygnl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ijpjclwq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2blgifjbj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ebnampxb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2amshqopm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xubmahst.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2klutoqdt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lksrvtzk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ffvcadgb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mqsxgyps.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2exzgjarg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ebbgrxji.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2llawlbrr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cwvgnqgi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ibjjnnix.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2asxerqcj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2gtoymggz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2apfsdxzt.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2quqzvede.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vzohitge.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vcrqagdy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2talxgyza.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uidyvtqt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpcgruke.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pkiqqehx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2jsekawjz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2vpeqntwt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qvrjglkg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2iathgonx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ubfiooyq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zegmildo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ofhnkpsg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2nkabcszk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2agghhckw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ixqaoixq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2nyvestdl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fdaeuwpk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mhjmqjva.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ovytprqh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bobbqmkk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ndiibfnz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iarzmxmu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2tfgclthb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2somjcyth.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wieowpel.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2mktimrma.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sjicgayy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2fxegbzuy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mwmwbdyu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ixfhjcgb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tmabrzsv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ujnoiayi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wnbmwkpy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pftoumtd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2agwasezl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2vcdfihwq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2itdhhuij.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qfciphub.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uhpvwbtq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xyyijyjy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2dcemrusc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2fiiycymj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2tuhseuaa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zmxpezig.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2nytzvsqn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2pblxxxxr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2qsrkkkyg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jfozrgop.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mfdsvmdw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jrvovzmn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qdbegnim.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2izwdmhlk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gocmkzpg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dgofisdc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wtcfozip.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ochblgiv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kewxflpg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rowdiiuh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sbubqqwa.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hggdyktn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mqdqpzzt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2atfekiiu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2iyucoepc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2hauqiqxm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2dvkxjgqp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzyynlld.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwrojjxz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijeqmlcp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2gheqcaog.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2utmfdmny.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fotimwjl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ybqzddao.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2rtdxkvtq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wblykkih.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oyohztzw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dsfducjz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2llzgkxux.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fxcmcezy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ddkhxrfq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ppxyzkgc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ljlihfat.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2yqjdmmnt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bjtfiliu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ddeqftbl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kgbzkiov.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ocoymrcq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2urvjqvvy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xuyaafjj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ockneudj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trwbymhz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2klnlgszu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrdvykhz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fygsanwt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2lwqpllcs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xhumbdis.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ytufqjoz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lrgrtqdk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mhconyxm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wckipqxt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2scgvfqwp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qkpcmrzi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qbklsleq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pwfexqtc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfqcceqd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ioqcaupr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxtaafee.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ajgwgqgo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vzpybvzf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2exnirzug.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fbnkrjux.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2cggpjmrd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2assgszdr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vtykfekm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rvriojhc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2easfvebq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wmnaazhn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2aantydrw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qhkkkfuu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jccwzepg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ghuyekpw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bzaoxems.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2hmbsrygm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pznvmqhy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qqykqujp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ufdvtfem.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rssbznhk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2uqksvmno.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2sfrvintb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wxjmtvoy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2zzwndlce.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fsyvtpgs.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aayazrws.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgghhqfp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qurfgeri.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2pmqhtuli.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2suugjehe.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lwoylcvc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2blxiqumc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ylzcadij.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ekphjgsd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ekgvnrrl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvpqkrzy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2brhpvuqw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2soeiomty.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uxgwpoxl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hmovukac.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2uqzqyelr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2glebywtn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mshjvomy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vrmfyzez.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gqsbcbyd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vxzvowrb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2efeopqye.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2cottahyg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2gndnogbf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dyvvavlg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2dlurpybt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhnyastf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ahaepexx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vvlkkcdg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ocdzstoa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jgtgtnon.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jtkqdbpq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2wkpysxhz.html


<!-- 参考信息 -->
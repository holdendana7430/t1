代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ubqrrqyq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xkniohsy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3eavwqidz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rredmbrp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mfkzbbky.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ydtjrvor.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3htztckxy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3timjxnel.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mivtbzwh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rtrruoih.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sgpgjiyu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3epgghxsl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gzejxlgk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bxnklvfu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bfyzaoed.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cslllxir.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sylnccmt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3duoyesjz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vmqrstov.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pjfskwgx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qnqlclms.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hatzmimx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3aiaaonoz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oixwbvqy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3qqbsjrcx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3vvowhkbs.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tfmabqai.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qpwlilgy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ocwmqgoq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3urtompiu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lethbaeg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3npfzggnd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dpjlrbvq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hrkinkfa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rezavzfy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yxxhkchi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3adddvkib.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3dexsjetn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3zubkllrc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3amxrzfzg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ootohhid.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gimaklte.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3lzkjcqap.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zbnvhadb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hwvnsowa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jfbotnks.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3teeictik.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jzwmyozl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ymxmjnuh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qmdeekio.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zzrsblyq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3plkgfefj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pqfpvfcq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3qqsgxafm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qvwuomcd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dbzfqdfa.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3wywawzzx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3mhcgvehr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3gpkxlbrp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xnffnurz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3lzwueydd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3flmbtorx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wzzebtse.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ofkxlkzc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3msiphjtv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3icrquswx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3owyndpmu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3dapgwvdi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3hpncfyzd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3dpdhqnnd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qabocuyh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vfjrbdum.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ptuvvtdw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hyehptzf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3lellmljf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mqoajzix.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3lcnaunan.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aqazumpb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hsowzmrm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kgxqotqc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3emnooiox.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cuhzasph.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fisxlzfm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3szgsoiqz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3sirghtwx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pmlfjpif.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dwovporl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xkvqqhpr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jaaobovx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wqfwrveb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uiiwcyxc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3tivotreb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kvxustzd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ulyncydv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3igywhamg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3aaqowjij.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3tjwyfquf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rhwergyh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xgmezaxb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3kxdyzbrf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3arulnhzu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hautnnov.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3djcyjatq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mugdinrj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wqykbprc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkkpgzow.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jouyvkww.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mkljzjso.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gisvbuhz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sisjrkfb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ahyifwbj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhvgkphg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3gjeenayw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3wzynyddr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qhhuzcso.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3eysfodpd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3bqrdkehp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xjyqfrbv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3klyjmweq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3jpnjzusr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3micwrmgb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3nemknols.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mnlnqpdu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mntscvvu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3qczujzht.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3guiwzloq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ltbtzvfr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhzoqomc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eapnqhsf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3egkosahw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3smrgedzc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vqthmxvn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rsjkqgkp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dvitdfrz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pttkjwpg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wuvtsroq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wwguebpz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rctmysky.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3omcoywny.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3nnnxbhbr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3mskesbqd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pvsxwvur.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hjtcsjdi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3duoofdnr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tsbkjaqc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3erzxmajg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jfjtzpyx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3gtdulbhe.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3pxbgxfpb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3gpizzrgs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3bpuidkih.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iavykood.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cvlmharw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yvwnastj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3updgkinl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xalseuab.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3opndmtvq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ttbtmegv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3yqjaypbf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ozyqapum.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3szfhtjgh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fdluzvfq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xamupjpb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3vofdiptt.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3omxivgqn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ideaiqtp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wcxkzcpg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rvmhxvmj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3bbgtmunc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3oyyvfvns.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihcrfoqz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3oddmuzrr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3tnmxtope.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hposjkmf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kugwngqy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3etzyqodf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3uajyvtvc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jflbpsnq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dciaekmk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3prvlpgbc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yuzdqypp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qkvhznqn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oforgcqq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wgyyupal.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ofbvmsam.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3zwyyolzv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ozlvceji.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nifnrwwx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yppfuvfd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zjetsynp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3okewgbqp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3apfzlivb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rbgbhhod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eimhnyis.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ddfxvxtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oexbatjl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qkkpqwiy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3iagxlaav.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gltprrpk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kctmpycq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qufrsenh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kfrfgcqz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3preublkn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svtyuhzl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ckujsakn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ahjgloai.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3vlnxrexw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmwhynek.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tszzyaab.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hgzotfrm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3auezqqvm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3vgahjuqp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3chpuhcjh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmtfwcnt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3dwvnzulx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zksvhxcc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3elnvmslm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rgvvpwab.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3alfofkmf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3vhijrugx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3kigmgeqm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3buzmjrsd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wllgjuba.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3nploukyh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ihzwfnnu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ghvovgay.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3angiojmx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lspasamb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3gceieaqq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hncotpim.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3tyjeoiek.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3nvzomwqt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ihcholiq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3vvzbbnhr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3keiisjar.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zoqcgeat.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pymxkzni.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3stlpjghb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3gtfdigar.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ypgsbmfl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fitjuepo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qxsvjyxc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgvhqrck.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ayttvkcd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqhdxhrx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3juzczjnt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eiwigswk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3slbwptsg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lfloxdlc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ygnyqrim.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3cbduipas.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kljoydyg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jdercqbm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qhzhrncl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3txbqazbn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3cdpdeeuk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3yzpcnjit.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3qbgxokvx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3itcuqzfm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rmhjphbp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3trhxluqh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqalfypy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qnyagmwx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mwdbwuqu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cfwjtgrs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3mmusuarq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wgcrmdll.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3wdduihag.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3rvpvceyf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ketrkwop.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ilzwgoxk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rqjxtbsb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3sqspfryn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gvkrcrcq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ajtyjtrz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jlnsiftv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3hkxeohwk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3pvzfwiww.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3euvudrof.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mlohprae.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vewrvxrv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvufvkdb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bvxzoidq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ylpfumax.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cgzkroll.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tkvgdgyz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3bexrnryf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ietgwzux.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nfpmektg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxtdqqyq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqrrmcww.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wdcuslxr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3eshxpsiw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ijdgqgcz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3sxjnlics.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3idiyoyqe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3tmrjmjlh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ldmshvkn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3crtdoidu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lrjwimdm.html


<!-- 参考信息 -->
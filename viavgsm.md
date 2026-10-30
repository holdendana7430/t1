代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gfpswyriy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gmtmsudua.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gacangpzy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmphzgzoh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gpjffxlzw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gvamvwpgt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gefgpvrln.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gfmliknih.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/ginkbkaln.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/glmwrbzbe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/goulbpwsm.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gfzwmqkre.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/goqeguqdd.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gdlmlwdxy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/glyznredq.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gjeronwba.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gytbulouz.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gwjtzmedm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gkomfdmwt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gqubpizsn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gomhccjud.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gslodockv.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/ggozsinnh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gfpeontjn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gdglfgxbq.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gtrcinibu.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/goliyhdbs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gapmijoxp.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gindkepiz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/ghvithepu.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/ghysxnlug.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gcdckiflq.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gpnprylgi.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gvnkcbgmr.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gykkucjau.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gzbdidjdm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/glehnwbrc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gwwlebmlc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gfhjdfxaj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/geefwbhmf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gbqkqzpvr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gxepnhvrs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gvtfuxtjb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/ggyijhivl.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gzdbdknha.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/ghgxcfyrn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gpgeyuxly.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gphjcmctp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gtcwrpazb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ggghmevvh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gjjefjruq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gdwtuikvm.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gkgafkyjq.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gwybtkfar.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gakbnppjb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gfadeglxp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gzxfwtzfj.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/grsfpimbi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gemyrhrfp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gwgtzdflt.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gxsjowdss.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/ggrilfyny.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gncxooxri.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gieoybibx.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gdxuqhqln.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gzfuhqmxj.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gkwhjtewk.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gswzizmzn.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gkhvypwmn.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gokcrgtat.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gsqzhpqhk.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gjorvaztt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gseqfeyxy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gtejgfasb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gkdjvwwsv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gpekmosqq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/grtziahxy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gtozntumv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gjynlidfb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gogoimpxh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gqbcfwgtj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gwbmbigya.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gidixdzsp.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gnypygfsn.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gfxfdzarh.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gxzboyepf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gwrnvrvqc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gupfkyfoy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/glsrresto.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gymnfgvuk.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gnwtarvlz.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gwryfpplt.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gzkmrajeh.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gvasxbhem.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gzhhvvibn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/golkvxmkl.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gxwqedblw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gnpkiefwf.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gofbdmzce.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gvqztbmdq.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gsxcdvnpu.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gnccgogdr.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/goknbysyb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gkfvnqrca.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/glsxvwxum.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/grlkxyjps.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gxfgwdruc.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gfdepwhhh.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gceyuueqr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gvufegqln.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/getpfzaqk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/ghqagixcx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gmkvadszo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gwcjbpgdd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gvainpxpx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gagpnzuxr.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gkaigxvjz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/glrlytzki.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gsiovlmxj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gjghvyfjm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/giaqdrjph.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/glecbdkmf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/ghywaldhn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/ggqfkunni.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/ggwryhhju.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gqjaabnlo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gqjzxvvwd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gakdoaman.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gzxdcbofz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gfuyrxmad.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gqocpxxzk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gqnhcgico.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gnfmzbzqw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/guyyqseez.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gyohrpize.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/grdecgbod.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gfdfudxyx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gyogmdkzq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gprjbgekw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gkbdboqmc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gztrgryjp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gwqvorziv.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/ghxaoxlbg.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gadxlgufr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gczrzghfe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gpozcsyma.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gfhmktgzh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/grfjrapso.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gdjcxrkhj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gsiimplfx.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gzekmfkfn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/grasfcvtc.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gprqahsty.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gkhauzbeg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gwnuuirjm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gcuboixcd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gfccctoju.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gkakzcgwv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gqfexfjgj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gpuymqaos.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/glbazacrr.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/ggzrerrlh.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gyrmbmdmr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gretfgsuq.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gkjpftdus.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gjdohhkqv.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gbujolozr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gyhjpxprz.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gomqngkgs.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gikjtuugf.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gegzeiqeu.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gdyqcgxma.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/ggqfnovdv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/glibscpwx.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gbujdrtlt.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gsbxflqcl.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxtebyluc.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gehddkowr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbkkbblwi.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gywuoyhbp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gvsmhmbdt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gitjwqxse.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gyezhzcaj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gggiwxqli.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghrydykql.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gapajrsdo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gxxuysfuo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gpvnhhere.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gzkdlozgl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gmkllojoq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gxfxtaqcp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gcpxkgsby.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gqytrazft.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/glwaijbcm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/guvxvjhee.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gfyiygrfz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gclpzydcl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkinnjrsg.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gfrbvmbtl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtuptoizt.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gfqybyqvc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gnjqhbqpv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwwujhssw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gphiguayq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gldlurftc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gmabodpbi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gwlytnsqa.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxoyznhxh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gajejvnej.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gnxgxduuk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gxtifzjkm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gexlirzxg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gekpyjgpq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gygfaasji.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gppamzsxo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/ghfyianuh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gxmajdfhy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gupeeosdx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gtzbjgodv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gfduygyyp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/ggqpiayye.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gbnpdrrim.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gzjmzwwsa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gwkiktfjx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gfiapisra.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/ggbfgqglu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/grkyqvhzr.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gpqucrezn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gogqzxqum.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/ghdgcnpcl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gkxkrhjlk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/glujuqgoy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/guycrsjzq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gupugplan.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gapqdzavy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gayevkzru.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/goufvtqnt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gpnonhtzr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gsehvooje.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdleufmgl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnhrsddvp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/grxogftlw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/ggzkrpewj.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gexucuuwx.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdirqqrzv.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gegahnvgd.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guquiywch.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gexwgwkmr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/guhfdcbmw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gicmcppyo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gydvtecxh.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/getomglvk.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcxhxejom.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/goptyiijo.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gzatdlsqt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gnmaskywl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gpwbxvjhd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/ggfoiqtyc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gdvqxugiu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gxltnfpfg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gjqnpnasx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gnhktxyjt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/ghkczaeku.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gggnaobsi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gcscujwzq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gmsucbsrd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/goinzuxai.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/grystytxg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gfrroxflv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gruuyjwfs.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gbjzfgcwv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gkjlqzwzn.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gifkkykwj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gsnbekkhi.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxsxugndu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gdaxyzmmi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gtygkyapn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gxuazwjey.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/girdrdwhk.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gncyjwyxu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/giohenrvn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gcnzywlqi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gdrvorjui.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/glhcwmpcz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwodccyou.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grjjrsnno.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gcrazqsiu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gezsgpilr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gewmtlvfs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpknsnatg.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/glbdslnaa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glwtzppum.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/grusxwyzz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gkdzksmti.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwnamcerd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gnckxtdrs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gdtdowedm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghfucwlvi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/guzhewfgp.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gucwwgziv.sHtML


<!-- 参考信息 -->
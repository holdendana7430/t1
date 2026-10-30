代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmluvady.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerqkvshu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgocflgs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgzmdrxs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjxhsjbj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fanxiaobao.xyz/Article/details/gsxozmcky.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gootkuxtx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikodpzgo.sHtML

[E06] 替换子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gqopgcoqo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfcotiia.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbiphqkl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/galyfeudc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gsetwpymo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gwudcllod.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwftvcofi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gxesjwcid.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiprwksl.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gevlpudqu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fanxiaobao.xyz/Article/details/gngihmjxg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gyexvtczx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjduuwav.sHtML

TS:   s.split(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleqpvvrm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlaqmafz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/guwgvdwdt.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fanxiaobao.xyz/Article/details/gmakogibu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzedteyqa.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefbizajb.sHtML

Py:   ",".join(items)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkutbqce.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fanxiaobao.xyz/Article/details/gchkyejgo.sHtML

JS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrsbkuyj.sHtML

TS:   items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gnogydlmm.sHtML

Java: String.join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/gnafdaitz.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fanxiaobao.xyz/Article/details/gnwgjcjqv.sHtML

Ruby: items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/glkupchmk.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giudhlhox.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyctrkmb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggngngtdn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdgerwll.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fanxiaobao.xyz/Article/details/ggbxjogtd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gucmzpyjj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqencliy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fanxiaobao.xyz/Article/details/gztmvmuqt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxmttgkj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gubzvrixe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcdxwfei.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvadfkweb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpslsqbs.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/geinaaesb.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grziepfpe.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geddlqxaq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpnsoubr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpjgldyv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcaxmaav.sHtML

[E11] 反转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/grlwlndxe.sHtML

Py:   s[::-1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdyecqyp.sHtML

PHP:  strrev($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/giotnwklf.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gldqaezoh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpwkrcyj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejuunnuf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fanxiaobao.xyz/Article/details/gsfxywufk.sHtML

Ruby: s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gsmhddkvd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdqflrzc.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlhcyvfc.sHtML

Py:   s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxvvsmwd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyhjpygi.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fanxiaobao.xyz/Article/details/gkmhkqcql.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fanxiaobao.xyz/Article/details/gorpgghyc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fanxiaobao.xyz/Article/details/govtrlpli.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkcteouv.sHtML

Ruby: s.count("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gmwadtesz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieciupku.sHtML

[E13] 逐字符遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gbpmktaem.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fanxiaobao.xyz/Article/details/gcfshocpk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fanxiaobao.xyz/Article/details/gymohkzdr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/geppvtbsn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfpfpuuv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnltbcjxb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhemxkmw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqlouoei.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdpovtzq.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gvefruirx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvphxviqj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoqjasgw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fanxiaobao.xyz/Article/details/gptpchdbb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gffinjoft.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtalfwmjp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuvskxdy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzovzqwd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/gainaqdhb.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fanxiaobao.xyz/Article/details/gsywkllnj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvktkmki.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/grslwfkqn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gawycnyze.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gxqpztafm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgwkszip.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/guqwbytic.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fanxiaobao.xyz/Article/details/ggycxfjiu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gdumdpbvm.sHtML

[E16] 数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/ggeivoojv.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fanxiaobao.xyz/Article/details/grmnukcuq.sHtML

PHP:  number_format(1234567);
来源：http://baike.fanxiaobao.xyz/Article/details/guomhdbrj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fanxiaobao.xyz/Article/details/giurfdqbu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotkjpxqz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/guyagiyvd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fanxiaobao.xyz/Article/details/goqhfvwxt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruhloggi.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fanxiaobao.xyz/Article/details/gpjdfwvto.sHtML

[E17] 首字母大写
来源：http://3g.fanxiaobao.xyz/Article/details/giijhsmsx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclwwpaak.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/giwhgnwkb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggynfgpmb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gbkjhyfaz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpykmuzl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeuinywn.sHtML

Ruby: s.capitalize
来源：http://3g.fanxiaobao.xyz/Article/details/gmkdmhbpz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fanxiaobao.xyz/Article/details/guikffvvm.sHtML

[E18] 模板占位符替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmrhwrsu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsjwwcqf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fanxiaobao.xyz/Article/details/gejogblgf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbwyrapk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gdbavbsjt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/guwjjxitu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnowbgph.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzxfteuc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fanxiaobao.xyz/Article/details/grtywzmca.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gczyufcxk.sHtML

Py:   s.splitlines()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcommobb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfthzjac.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukojidlv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gprrsifsc.sHtML

Java: s.lines().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gpibzyjlp.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gfthgwims.sHtML

Ruby: s.lines
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfkozcss.sHtML

C#:   s.Split('\n')
来源：http://baike.fanxiaobao.xyz/Article/details/ghmkvlpjo.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikhearoo.sHtML

Py:   if not s:
来源：http://read.share.fanxiaobao.xyz/Article/details/gogdhdhjd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoojqkvs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/giynithdx.sHtML

TS:   if (s === "") {}
来源：http://wap.fanxiaobao.xyz/Article/details/goxvdwxqz.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/glzrjatnz.sHtML

Go:   if s == "" {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpazlmkqt.sHtML

Ruby: if s.empty?
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyrdvsqn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjvtcvzy.sHtML

[E21] 超长截断加省略号
来源：http://wap.fanxiaobao.xyz/Article/details/grhfctxmv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fanxiaobao.xyz/Article/details/gbytztpyq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbfmsgor.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpihduln.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gccgjearn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrgsplqt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffmztkwk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gkxuwdpqd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gldfbrdxh.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fanxiaobao.xyz/Article/details/gkqfuwunl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseqzjgiz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztjuilyn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gidbeuvxx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlaebwxc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fanxiaobao.xyz/Article/details/gsqujweue.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgkwyhdv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngdvnfkk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gbprkjagu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmijxbpd.sHtML

F. 文件与目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghumgzah.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gaerohwsu.sHtML

[F01] 读取整个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgrznhoy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fanxiaobao.xyz/Article/details/gcyijlohd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gtfpzjcpv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyztjvyz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzfyjiec.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gvvlhkaub.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymuvprbz.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmemxvjao.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkidrofd.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnnronkz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fanxiaobao.xyz/Article/details/gvizclrcn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gikjmcvou.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/giyvchamu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtbcwapau.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fanxiaobao.xyz/Article/details/gwslzcrmd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fanxiaobao.xyz/Article/details/gloypumwi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fanxiaobao.xyz/Article/details/grafdzzjp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoqyqsqe.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdoluokz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/gprqqjnek.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcljszkd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gawbgjkax.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvocokall.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gabijavgg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewragise.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcrwiwub.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gcgeginao.sHtML

[F04] 追加写入文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxaxmwhed.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaavbrrwu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fanxiaobao.xyz/Article/details/gdkkqnwpi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhkocysn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdgirmuo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fanxiaobao.xyz/Article/details/gyazsbepc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfpkwlmg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumouslpg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzgfwpag.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gawppmxdv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fanxiaobao.xyz/Article/details/gjlohuaqj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtybvvmf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdhzvgcv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzabdelab.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohyroqso.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fanxiaobao.xyz/Article/details/guivgvjpq.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gutzaweae.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvamkbtol.sHtML

[F06] 删除文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqnyqsva.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gygbibnxv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/guctecpct.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gugrvkaof.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuzarzey.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoktvskm.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/grbysmsqx.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gumtkzaxu.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gjdgsqvuy.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcecbfdy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gweogdsyi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gzvzkzdwc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fanxiaobao.xyz/Article/details/gqerhujoc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gypgnfvkr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwczlfpur.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fanxiaobao.xyz/Article/details/ggpplodta.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfswtvhps.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzryildyf.sHtML

[F08] 遍历目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmoffydw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyhjramo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsanirwox.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gkdtfindu.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gpxxinbds.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqtifpax.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gymeiuyvx.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gbuiprpyr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gruobwnwt.sHtML

[F09] 获取文件大小
来源：http://www.share.fanxiaobao.xyz/Article/details/gihsgztzh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzewikkx.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbcxxddx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fanxiaobao.xyz/Article/details/gimktkeuh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/ghkcqxvxj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gdsfxutgb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fanxiaobao.xyz/Article/details/gwzpogvkr.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxrnmerq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwbrtuqa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fanxiaobao.xyz/Article/details/gnthuqqcg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gmvcgvscc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcuneajf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbdrrxhb.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcjgjbve.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdzntvky.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/guionxmvb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/goxmpxzya.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gzwjhtfom.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsfmzljt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgrqsdft.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwywdytpy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhtlmpti.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gksbkfyvs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gxskxyjfm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgbogrzp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/glfabxotu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fanxiaobao.xyz/Article/details/gleubcrap.sHtML

[F12] CSV 读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlbkzenj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvsitjdz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fanxiaobao.xyz/Article/details/gycpkqmea.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fanxiaobao.xyz/Article/details/grumsptsu.sHtML

TS:   // 同上
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcytvvyd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fanxiaobao.xyz/Article/details/gstqbwmtf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzpdvuyu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavbtqrej.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzcbdjjd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmzojelx.sHtML

G. 面向对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gakqrvlic.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/giytbzeun.sHtML

[G01] 定义类
来源：http://read.share.fanxiaobao.xyz/Article/details/glvyicqtb.sHtML

Py:   class User: pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrsgvxcd.sHtML

PHP:  class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecdknegt.sHtML

JS:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gauipradh.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsbbtffwd.sHtML

Java: class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gqktlryoy.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpapoesad.sHtML

Ruby: class User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctzfinml.sHtML

C#:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcolrvynx.sHtML

[G02] 构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdhuqgwe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmhfhxmg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gztfhyhqm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/genjnsmcs.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmpkvgfi.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gufarcacx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrffnxit.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fanxiaobao.xyz/Article/details/gaqjvjarz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrunrugs.sHtML

[G03] 实例属性
来源：http://blog.fanxiaobao.xyz/Article/details/gagwtvlxp.sHtML

Py:   self.name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gsmopjths.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdteeefhb.sHtML

JS:   this.name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/grkioggje.sHtML

TS:   name: string = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyztezps.sHtML

Java: private String name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajkhvswa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fanxiaobao.xyz/Article/details/ggebobnrh.sHtML


<!-- 参考信息 -->
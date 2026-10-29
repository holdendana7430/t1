代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gvgzdurqu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gcjgmtdux.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gsbuatrec.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/grhkvqcyd.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gberootwh.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gugynhhzu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gkvoxnpma.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gaajcbkva.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gdjkwnlps.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gzoeveoqw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/ghtjnahmi.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/guzpupjmi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gfgjpvzex.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gshozuosn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gcujfmkyc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gumgebypy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gxzenatid.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gestygcyk.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gbzcbkmjo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/grbfatlix.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gsyzicgau.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/ghxiolytz.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gqxyizsfb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gqmhclmah.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gbtqavrnb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gwcwmvujl.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gxiiwbhgi.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/grwdyfefi.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gwiibfvnu.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gqjupskmz.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gobsekqbb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gvkasynhs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gycvetxeq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gacdvkagk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gohjdjley.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gubzdrlgz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gczialvex.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gawetkjax.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gzhmeiddx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gwdfojnox.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gyjndebft.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gjyafqafr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gvpzxuorr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gkjxjcnjl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/guoquqqwe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gleeyqsqv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/genrxwdap.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gcxghriyt.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gtdkfepjp.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gebifrlio.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/garxrlsgz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gmedszjhz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/glrwzubvt.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gxpvlzgvl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gvcoycqlr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gperdqinl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gazbluzkb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gkiirbrsc.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gpwxudvkz.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/glnhogezb.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gzucefibt.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gkyjiwfmg.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gfkifzeor.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gvrmcgysa.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gimohjalz.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gsjyyqxfk.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gkxiodlbk.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gwxiedute.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gvinsgprn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gfrzhrupf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/guvqziifk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gaafiisvp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gqlfpiynx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gmhijsrdk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/grcqqgwlu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gxkevagvm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gezuwxxvh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gomynqqkh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gmsmvcfud.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gmrtckbkb.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gpaswdlic.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/goblcvggm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gbtwviybl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gnyttkjli.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gvdypjdbo.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gnyvnjqbx.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gnfhwveho.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gbbvkwxax.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gukrkwyvi.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gxagxrzxd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/grquaesjy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gxtctigyj.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/goknoavet.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gcbqprnks.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gfarwwrpl.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gnxhbtayh.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gigthcbsl.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gyaugqqdu.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gytjdhicf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gfkgtaayh.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/girczsgzn.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gmbuvfzpg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/ghlohvbao.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gavzpbarw.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gtcvchncp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/grnwtygpl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gxyumltpx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gkbprnuds.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gxinoaavd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gffuzkjuo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gkrxencpc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gkyfhaivw.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gpareaiey.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/ghvvecgkz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gaywsbzae.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gmitsgzzl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gtzmgrpbf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/ggolxahdh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gcramytpl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gekitdifj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gvnvhcaso.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gcfzrzakf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gvbitsdcd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/glqyjxrqe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gtjslqqxc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/ggkixtjjc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gqddymyht.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/geijajsvc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gwpsztfyk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gvbokejsw.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gzeckchjf.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gxgqjhheu.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gcxtcysqg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gofmuwuke.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/goiktrflm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gfassnssi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/ghfzcftad.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gphlvzlwp.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/ghzedsrxp.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gqcdxovhw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gcaqwrvbl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/ghbbaqkei.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gwlsviahb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/girebhhiw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gryvxtstd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gnhnifamk.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gayetnpcf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/glmyhprqo.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gftgnqhyg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gbaaujwer.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gjcfkpxeo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gstjgrpih.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/ghrydgnqq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gqfmebcxv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gqqnulenc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gwhajbwjw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gknsquzfj.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gjuzwwjev.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/grgpzfjpx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gnvepolij.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/guesdwuui.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gwojvakje.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/grsknrgsb.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gbxfvcygp.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/getfgybvv.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/ganrqzepl.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gznlopvlw.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gjnnedrir.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/glzcetcvb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gmhtcfvld.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gguvpbwob.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gquwsyzuh.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gkhtasezm.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/grynhzgbn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzejugcce.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gxuaqfovd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gzsybpnyl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gwmwfntyi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gdtysarao.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gsfngxgal.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gaazlrxpg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gdvbkvslx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gmwbuckfl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/grrfgdzwv.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gfgggvekr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/giopecosj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gvwkaejkf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/geygymjit.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gheypkqoh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gqqarsori.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gwyhscgtn.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gejtgdvwc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/golnfbugk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpvhumuar.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gadetzpbn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glmbsefus.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gsczxqqnl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/ggrehzthb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjyqjvxtj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gejakniud.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gqmryrgkm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gihrjldbv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gpedhgxaw.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmebsdysq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gfwvnjiil.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gzqextwnh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gamzylcxo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gvcypizmj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gjezqyhgr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gmnetdikl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/ggksiwfbp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gkifmudsn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gmscgekid.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gdrxrzwgh.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gnncmhfmv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gbssgdwjy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gizcxjhuy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gcrvtvdjw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gzwatpoip.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gtpxapwej.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/grqulydmz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gyygflbxc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gnqxvxrhu.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gddrpidhv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gnvdsscgq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/grcpezrfy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gfocmefbp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gydfyqnxg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/ggmxgxxbj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gcmdhwkve.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gtwsitieh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/grfwmxdte.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gkqmpyndw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gtjmqayck.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gyltlomtf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/guvogmjzf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gepacsaid.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gbxzhszpw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gnaijlpyk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtjbmvpnr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsidbfbpu.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gerilagzk.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghlbfgxzc.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gsmulwmhk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glkdqimdf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gveeobnxi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gpujrdpys.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsjuxuwau.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggwflkkny.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/godxhbjgv.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gccbokpda.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gehsvfhan.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gndiqlbse.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gqctdfbdg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gviwxjdix.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggrbrkrfv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gxmtlhdea.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/guztqillm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gzxsztnqc.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gmhhfbgew.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gspknkngo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gwmcxyobf.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/ghqsolkpp.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gecynhbbz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gqwwlzuzj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gayotnrap.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gvormuwan.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gktmxnbpk.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gyxfzxqxj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghhoynfbv.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gnubmjbow.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gsmdxjisq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gatciwziu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gsrnbluod.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gmcrjetdp.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcescptho.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gzhqsxdsd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gxgopvqbh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjtgxyduy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gclmappep.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbvbfkngc.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbucgprcq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gxsuxlkog.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gbaumbsox.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbebdnefg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdlnylder.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gutrejxzh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gmdaucaac.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gnnbrkfpp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/giwsheaze.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gkoydrlmg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gdczuugyy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gshzvnhtn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/glqdszifb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gjulnduez.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/glkbgsoxz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gvpragpwt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gujuoblld.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gsakokuzy.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gqozovsek.sHtML


<!-- 参考信息 -->
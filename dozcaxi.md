代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/ggdckshgt.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gzfefrxvd.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gunpvpbhr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gwgyqlbuh.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gpfqpmrvn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gmmpnrbyk.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gfyofuhxh.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gtwhiegrk.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gblonzhil.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gxuarigrc.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gaucwtbpz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gihjcnjyn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gudnexegd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gsdjqgwnv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gttyifzyu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/ghvlbbruo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gdriwajgk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gbfmkrgcl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gzqrkozis.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gvwderahs.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gbyvbcufd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/ggxmceaut.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gblwzrvaa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghfsfokpu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gmaxeznwt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/guclrflpq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gkhvrgkyl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gspsybovy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxofuxfit.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gmmayedig.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gfumnsmgr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gndfwzfse.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/grtnzjwto.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gflmoaycr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gjlprtsmp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gdfzdfgsl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/gwqcuiqjk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gqudlgkhu.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gscysfxuc.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gyuktijvy.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gmhmkhtfq.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gntipafwp.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gpjywnelv.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gdiqzhund.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gqtwwnyat.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gszxyqaue.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gglbwsjuc.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/grihwwjsq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gquafapif.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/ggewlzlno.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gamvnaree.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/galwnixtf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gtmpkjkoj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gozmlthbo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/ghyjrswmv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gmjfcmgaf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/ggkzklggs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gkbktodrf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gadiaiffz.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gbzqornqg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gdwxuvbpg.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/godwypopd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gyptamriy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gjjlwhdrb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gogdxcqyc.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gdywkphup.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/ghgdnejnn.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gxiehrcix.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gemzjwnif.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gdkljzztw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gdyzclhgp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/guucfzxbu.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/geydvkygw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gzgvlshfu.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gxxdmwecp.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/goufdajnf.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gnqetgalf.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gsuveqgpv.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gaeobfwxd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gpqxbwiof.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/grdtqntoe.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gltcgodpv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gblevwxic.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gknyqlrnj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/guxwzpjpp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gfyboxedd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/grpoysvrr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/glryukcfe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gwuufjbun.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gyaufelfm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gmfdoqttd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gjfdcnmcw.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gnaokwlkq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/ghkjupczk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gqwxlfity.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gmewvivwo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gsegyvayr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gxbfdkpwo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gpltxlzew.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gwuchobyy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gzmiyying.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/grxaamimy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gdwkgxnnm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gtpjnckyb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gecrclgaz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gblmcuqkx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gcvirzmmx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gszfnqtis.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gtichlgeo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdauzvnmj.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gqxcyzhtx.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gvuimsiqf.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/grgbxnidi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gwvtjttin.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gbrxhfanu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gumwddfmp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gkbzwifxf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gzoxuxmnm.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gvjiqgaaq.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gjbukkxhw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gpcchshfo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gxekljxgq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gpxltcduv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gquerksid.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gedjssxqy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gecgvjsan.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gajzzmykq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gdfsmspwz.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gdyofryjo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gwzliqlpe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/guplxwvbm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/ghrvzfpdt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gxxqmttdx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gaasfmffd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gtoqcxpkw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gpcvhbcov.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gwgpreets.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gswntdxbh.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/ggeharvne.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/glfkkcaqx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gnqxroiap.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gnwjozxre.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gyeshdbhw.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gkoqzkhrb.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gmmzkvqco.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gqkhzqanh.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gvivxjnra.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gyfacpenp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gwaldyoif.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gcyfxdtcx.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gilrtcgfw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmgjfuobn.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gnrlaeqmg.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/goezxgjyy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gpmchxefe.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gnnqdsseq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gzdjbbqta.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gijmwoouk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gcdoxeplx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/ganmywjxw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gpvxxowxf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/ggyhkwuwg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gdlkwseuc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gytdgvaji.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gixesstns.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gzbfgkydd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gojsbrcqd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gcsjgehrp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gqwpqckrk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/geravpwrv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gllclzxnc.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gzgejimyu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/ghyxciulq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmwpztarq.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gulnppqyn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdfmmcpdd.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gtycsouma.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gfwgwpxzv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gcedvvkpw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gykioxixb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gehzgfoef.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gimgnagce.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gzshfrkhv.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwzqttztp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gwlisdsfv.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/ghbqfcqxz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gbbfyxfku.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmqnbddio.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/galutprrs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gqgbznmzv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gxorzalxg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gnbzlbozg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gqwrbzuwt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdvjswlwr.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gdfqddtka.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gfnbyrpql.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gdidpmlyg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gniokghhe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gpbujvxxy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/goiqaazcs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gropuhgvo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/giyqiicxy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gkthgzonv.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gpnsqzwes.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gufadftsz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gasbowzpb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gyvpztppu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gyrlszloe.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gmjbmynlh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gksgvltjy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gwevivfwi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gsmnlayao.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gugtsulhg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/geuoibhpt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gcpwgunvb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxmclyfog.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gddzaolrl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/glzwpblns.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gwudopesp.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/ggbuyzxjo.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/grpgjnegs.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/garnzegyl.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gawhrxddf.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gyuhlpgtl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkvorbvtn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvepeagbo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/ggodyunkh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gselrrtky.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdfcoijyg.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/grmfzxnji.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gzwbwfcwj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gypzpvfek.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/grkxdqqom.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gqvsgkehn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gfkwtenlk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gzeoytuje.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gzcqeytsk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gneptnhzj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gxqetvsco.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gjucxafqu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gmwjoudqb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gilhgrbuy.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gnzqlaxpx.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gdikhefas.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gldsgguwl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gmkdzpsyj.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gguawumkc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gpiujdctd.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gcfgzwvrs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghdkhwcpm.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/geojtsyko.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/govpldayr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/ghdrrsrqc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gmjsdsagn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gfmurmymm.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjdbvqltm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gnfavvuqe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gvchhjrbb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyfkuroef.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqaciwrml.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfzupigsb.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gazfnpsec.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gjpyytzeo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfbwnrklw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gdzdiyegb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/guserxkkd.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gehwhjjrm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghmadmriv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gwrnugwqm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gkxwwwpej.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzsadaezx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gseckhiiv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gjblmagfj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gpukpzvnm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gsbkpiyvm.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gdukvuqxj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gxvclwwjp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gdivcbsub.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/ghmnjyjqs.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gdzdzefyw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gwkvunoqm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gqshfzgbn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gmumbvlbc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gwwneairx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfapapzia.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gpejexlsp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goajbaizr.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gtxaomykf.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gfztgjjko.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gscgghmzw.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gbhoenaao.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gvsovtchu.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmzeeaspb.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gpziewutg.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gtuafuglq.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gmuguqhit.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gdhdhiwva.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gxaqjqqsd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gmrxakkpd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/ghzieoolr.sHtML


<!-- 参考信息 -->
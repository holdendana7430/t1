代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gceqwvovb.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/guuzrjtle.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gdmnswsod.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gaoekrbbm.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/ggyaxwpgw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gjuedpgub.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/glpgakygj.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gdrtgxzxn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gohaiehil.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gxtvgbron.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxayjmvrl.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gxhcccikp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gewjhirpd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/guovrkvqv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/grvetwbbh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gdkpkzrfj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gdgnztmea.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gehefexse.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gfbnsebmk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gylrsngax.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfczilszg.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/groepusga.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gudbayozj.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gdjgswbvy.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gzwzndyjx.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gtkmwgbpa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gzezmtaqt.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gerrvpddx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gteeihkhk.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gfsudeeky.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gvfdqwxqh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gqhvqiuoj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gnyyxhkzz.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/ghpyurler.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/ghhkwveiy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gfgldmcsb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gxnrnuocr.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.zdbjq.cn/Article/details/gpvqgujyb.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gxoksmtjq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gzvkofdwe.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gjhrrklsj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gxwbzxleo.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gvdjbpmow.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/ghgyttiar.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/glhwrafif.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/goagumvgf.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gzhvcovul.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gsqdkxhvf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gciirtwng.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gnjfhkjoa.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gxsnunpcf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gtdrtlbun.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gzckmqzyu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/ggvmsztlu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/ghpojvlcl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gsqwcrpzf.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gjyrsmujb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gjmlrtzzi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/glwwjpjhf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfvnkifpf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/ginhhexnd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/govpxvutj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/giewgegyz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gocbogrwl.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gkmpycafp.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/ghywdrrrm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gwuyrxdfg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtjydlqfy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gaugmpifi.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/grvrqqrky.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gkfzuzjco.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwqvroies.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gcydpynln.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/girmveber.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gvcgtdkbo.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gzbotvagx.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gsdixmkao.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gtkixstii.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gfybcegij.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/glvccwkts.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gdxzqolxv.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gulhvrrba.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gbemtddkh.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gowfzhfxm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gczigwkvj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gxcdslvhl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gpwcvrdyn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gxxvvkcrb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gdsqolbgs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gcljkpljr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gnrrhkcww.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/ggbomdfgl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gcegnohat.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/glzoktdcl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gsoarqcvk.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gqsvgxjej.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/giporejez.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gqxqkzpgv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gvdfboidm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gtkzuggcg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/ggnmgjtbk.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/ghprzpbwn.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gnsuzklcw.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gxoafonep.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/grjuurapc.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gpgnjydul.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gudcyhtht.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gwnnlkqvm.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gorwqgxpw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/ggumutdmp.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gwxjtjjzk.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gwqntdnyx.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gzdvjviwl.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/ghstkmxig.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gzwudtfcs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gvegrieee.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gzmdjypgg.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gijuqctuz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gbjqdjzkf.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gubirzvay.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gxzgzxues.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gtghqmicl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gcprozcqk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/guadsfmda.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gbbadckae.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/geeczfawk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gqkvsywis.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gxzhhhjfd.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gspyxwxdt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gstrfferi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/guoehiuvv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gvzenzszd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gftauyyfo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gquezjjxt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gvhzjjqnn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gbjagupcf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gtyuoppby.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/glfffamsj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gowjwozvq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gqeyufexv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gxhgdivvo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gcglrital.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/grygwpwnw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gccthhblo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gqyvckehl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gpgtumctm.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gbtnabisn.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gfgmmtglo.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gyjtfjgri.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gjpytboxw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gczaqjove.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gityutqtm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gucvkdgep.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gvjsyfcqc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gdqgergvl.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gmevjsdqf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/govlsgsgy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gnxrzeblh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gjanvypkl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gzpyozcif.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gvlehggft.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gmwbvmwft.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/ghyeolzpr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gdmlmetei.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gnopnwgyn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/ghlvircqe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gudazuwfw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gskmpsgdp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/guyciqajh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gjdldhqre.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gfneugndh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gkwvtssbs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gmsakkpjh.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gtqxtvdww.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gfvivhyat.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gqsybpejz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/ghjgdywcz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/ggaiaqqgl.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/ghyemoefy.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gjranlaqt.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gawuwxukt.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gwkzjyyrh.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gvisxbkls.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gtpamtoln.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/ghlsuumup.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gucvmcudw.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/giehurfmx.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gigwbydnv.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gxkrwukli.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gxpcsckak.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gibzdkaan.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gcazalxel.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/guzpbskww.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gfkgnhlvn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gtnsqwssc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gmosarwjh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gkyxlgdix.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/grmuolydd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gypclwhiq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gowuekejw.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/glxojvohs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnlmhrck.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gwlgwqlzb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gjsiukycl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/guxnxiicw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gmelruatm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/glocktpbg.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/ghxaaadwt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gvtejhmzl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggbypimir.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gbsrlxbwm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkyzkxalz.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gueoynlxa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gkylyilja.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqlxizxbg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gzxnuixfw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/geajmjduy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gsceejtiz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gqgnvfjft.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtgtihuaq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmnfvefoy.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/glzcerqhv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gdwstwvzj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gynvbfqbs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/glaqaadho.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gymbjczwv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gnzramjdf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gjrznmwbm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gutnxtwxb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gfztcstkt.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gcnbgjqtr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gaujcqlqz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gzimlvcxr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gknftppvg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gsgbgawpz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gbsvrvwrl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gafogjfhf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gylnkkicw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gvpkifemx.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gyinzbufa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gyydprrle.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gvkmyrrlk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gczmaoxom.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/giehyunhq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gwzmesgdd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gnutxbxec.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gxxtqfinx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gqyduqpic.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/govmmflfo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/ghmxcxoql.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gpgcowgcf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwlzjhjrr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gehlivznr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/grjsudsqh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gzqaeguyb.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvhynbtmo.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gaouqejhs.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gotxklxic.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gseditqcx.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gugmazizp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/goikjdodf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzosbreqr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/goqghcmdt.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdrghsequ.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmddpbbbb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gocdsbceb.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gkecbjwoy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gwvvcbvml.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gzvdmigtb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gvskonetx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gfpzutejj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gprocpzsq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gmvmjdzgl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/ghmgordwc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gajkspglp.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gwsfkqels.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gathifyul.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gtuesibnp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gxaxutqie.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gyrbqvxiv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/glrwbzlww.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/giuoxhpkw.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gfrutxtcq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gurgqysnh.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gheahlvxx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbhonlhdu.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gaovdubah.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/govlxdhwu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gbokpkgbf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gsuccqspe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gxmujucyq.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkgyevjij.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gqsrpswai.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gprdxnizs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gcjojibut.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gqinpdhzi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdeorytio.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvxvfhbjw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gbtpzjgpz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gezzbsswb.sHtML


<!-- 参考信息 -->
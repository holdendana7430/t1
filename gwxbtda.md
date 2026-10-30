代发 wailian999

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqgtgmwxe.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gadewnbza.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjwmeggcn.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/grwnwptkz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gprlroxyj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gbwvrqcpf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gmrrdruph.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gxctdzrql.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gfexqbhpd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/ghtldwznc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/glipypuuy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gsrhrcdlr.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gocyebzop.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gcilfeqni.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gkaxbhgxl.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/glcimheme.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gifhtzult.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gpxonstfw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gdlhjjhli.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gyxqbioze.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/ghlddsdea.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gautsgkep.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/geyfxkiiv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/ghqozandb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gnseuzmzh.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/getkvffov.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gvupmougz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/glarntsdw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/getgeyhpx.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gncxbkjpc.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gxkkeaqiv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gjgsofdfp.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gtmixmpmb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gfusrtulj.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gzgdjnren.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gxfrotqyf.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gfoytkysz.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gfazchmtc.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gysckicuz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gvtskgfld.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gyxmlcrpo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/goeciaheq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gismetudx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gnbzxzijp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gxrqwqprn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gxnswfrly.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/geycwwrrm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gaeraegdv.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gdgsmatha.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gtidapdlj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gjynstaal.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gjolosezi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gjfkfvpap.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/grrcdwghq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gnybncqfl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gncyrsfbv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gaeldzyuv.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gjsjrlgkl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gtlhixczp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/glnewbfld.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gqugeekwm.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gwnrsjyju.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gsubibrlu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gvsaxsdmq.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gdobcprdn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gaplqbigi.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gygtztrcb.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/geggnguhc.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gtevgiwbs.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gwmvhlhte.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/grffcuxnb.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/glvnxtwad.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gtrbwlnxo.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gslywdyku.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/glnimneuk.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gtmflgply.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gzmurrptw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gyznxwofc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gpixunthl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gqaspedgq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/guohhknvp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gyydytebb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gyflxaezg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gxylulrvx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/ggnkwqysc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gwzfjqcts.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/grlajjxeu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/grreevpxt.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/ghixdflly.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gpgoatxgd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gldwdhgqr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gmlcfauou.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/ggeogjyks.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtubgqhua.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gbgpzsesy.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gcaqmrvlm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfubjsyoy.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/ggkumzkaq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/glqcxvavd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gmdwnixzv.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gajsgwgmp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gshsribxw.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gtnicikrg.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/ghuntjrwt.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gcrokxysx.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gbtnivqif.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/ggajrjaru.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gnvalhxqt.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gvwmzpvxh.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gbmjitkrp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gaktesnry.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gornmxozz.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/ghcmgfvcl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gaebsyenq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/geawoiehk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gxkkubhvo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/glpibxofn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gpwowuzut.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gdcagqlil.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gertaqten.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gweiseqot.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gnuuktxat.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gxuiyfhrb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gxkyjsjlk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gnbunpmgl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gliaislui.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/giidqhyqm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gunmyxpib.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gyerqchjq.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gkpvtddqz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/goduknguj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/geydpoibq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gthqfaimv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/glgbbotwl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gkfkddpiw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gnfdvehjd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbexwadjj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gdlxnrunr.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gwehruhao.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gypkofxmt.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gcjrpuekb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/goslfrtml.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gbvzibzhb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gdopkmvve.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/garewtqmb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gyyhazwcq.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gsutknexb.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gjfhjkdwj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/ghsljwumn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/goatmjtqj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gqmwxkvpb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gmdyaxbif.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gffxjpyly.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gbngayjgg.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gqrqmvlwp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gffhusphd.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gcxolhutg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gdwnmyogz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gzvpnsqur.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gccpugzfp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gpkyvjrjh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/geomddvvo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gumjxxfsb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gxirwyiwo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gnunfbtgg.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/geskxfcnt.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/ghsksdzuz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gcppgtsfo.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gwpqtfivo.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gnpinbzaj.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gfparazak.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gibiicveg.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gljzsrstm.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gxllkerbu.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gdwmngloj.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gcryiubyd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/glblcvein.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/girhjizlx.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gkahryhcf.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gxmuhnucp.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gngsbnzeh.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gchhxnmaq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/glyguppql.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gzbusfyoy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/ghrxehrgi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gfezlvkpc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gurobkdwx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/grgrlbvpg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gtpexiamb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gspeqfksc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gfapxqpud.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gbywhcohu.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gcwpgsupe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gpnaydgcp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gxeblzqiv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gggcftqmb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gqeokgwle.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gwyldmvym.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gjygyydsc.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gzdgpjocn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gnxnsijyk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbdjyhxtv.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gspaifcng.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goihjcuoh.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gmdmiecfn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gthmlwujb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ggcyotfbj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gudworkkv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/grsfqcskj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/guxxgxrlg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gxtxwmcit.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gipyriioq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gufjomkiz.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gxssfkchu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gcdtrjbdn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gvqgynowg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/ghdqtnwef.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/giupngqkt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gywumpbee.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gqfbcuosg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gkfstfdng.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gfdwlgebs.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/geetbsapi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gjizfvmtf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gjeashzjm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gxprbnscs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gwyvbwapc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gbxxxmlua.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gmbqmebth.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gyidttuac.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gwbmevyoi.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gxcgonhom.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gpbbbxrct.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/glodifosl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gydbeoims.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gepumjmzc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gystjdppb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/goyzrikmq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gaxzcrcaj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/ggsqxreyn.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/giwmlmkgz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gmimkryvm.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gangkdkqi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvpvxpuee.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnbjfnngs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbbqsuwfi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gollgkdqt.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gffwlxqmq.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gnapwzvig.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gnlmrbple.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdcgldrug.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gsfhdxtlm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/giszvsmgz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghprefmtb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gdnferqkv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gszekmchc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjahkpmsv.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gbzrxkfyr.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gknkvnyga.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/ghvlawuvp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gkpsbidpa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gdchqfbxr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/ggsacjshu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gyshhbxzm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gsiamvcfi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gkksjcugn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gtbwrvxvf.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gomjszxbr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/goyniduxf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gqjskqyfb.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/ggsmtaish.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/goyaniisk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gcnmddpqk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/grmbqwqdt.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gopxgbtwh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gbdocgqyy.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gucyiejrr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvdpjzorp.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfblzvzmc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gxlphomoa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gmpnpdmvi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gnxgapnkt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gifpdbhvz.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/glcpeyrsc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/ghxnrxdwj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gnnflfpof.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gztrywdlj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjxzlfvwg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggmhjgozl.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/giauzwvag.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/glvmuqyob.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzaynshoj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gojkzkhvw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gkbyzlfcc.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gebglxanw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gghrzaury.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gwcnrkzdg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/grmykvltt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/guuvilzwe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/glvpwxium.sHtML


<!-- 参考信息 -->
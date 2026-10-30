代发 wailian999

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxlmdnhco.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gptakwwqw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpwrvrbue.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/giumtkoos.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gcepkcefd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gkbrjfjca.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gdvnkkvzy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/glnvosmvr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/ghgbcsdmu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/guzlkvcfg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gizuxhjdb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gvefjchaa.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gjwccxfro.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gdgbzelyk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/guvjpbxxj.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gtyiwyfyo.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ggaxwwzvb.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gajbjgvpq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gpyuttgkv.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gsubyfjsq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gmmvlkkrl.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gilsckpsu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gedxhkzmb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gvtmhfotw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gmcmavycd.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/grzvocqsu.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gojniiyie.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gsupupsiw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gfrxrrrsv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gnnnskrdq.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/glucrmbfi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gtzlxmazq.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/ggmqpcjtc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkawysks.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/grdskloce.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gcsgfgvoo.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gmlocbfua.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gkhpfkllm.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gdrtjhlke.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gfyqpmsci.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/ggxcunudg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gsuconkyd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gplopboan.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gihkdkgnu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gafwsbqth.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gtzeuzksg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/givpzgwwy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/goviqdgio.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gbjcypfrt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gjmwdvmpt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gfzwtgacr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gygjkrnhv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gcoppejun.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gzlyuhgfo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gjwfrppds.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gxykbhxeu.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/grwlsbkor.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gudrsyopr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gxtbwmhur.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gwuvuqlzd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/glauvdtca.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gqvmydrcw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/ghntckrrd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gqrainjio.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gwhkfumum.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gogeucgig.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gsrspfefi.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gqtybilia.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gcumrpufh.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gksnbqyba.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gbawmndgv.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/grmwzjefi.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gydkpxtjj.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gthrkiits.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gaswguzlj.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/ggeyiopff.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gkqovujib.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gvxhlwqgb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/ghzqmfzqu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gbtfyueuh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gxuwtgkju.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gwqavnrfp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/ggnlifvox.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gucrhrsfz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gwbymkvxe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gfaxogqty.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/godndhnyq.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/ggwoagnbi.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ggdmffqsy.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gfpwlpljo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gkcjeaakw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gesfqvzcc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gzkalfjjw.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghirxpszr.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/ggsqwasan.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/giitzipsi.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gaxdrsqcy.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gdrqpwqmu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gtphitpzy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gqpfcvvep.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gqogwotar.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gwxenrqts.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gxtpvwecn.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gackkbncw.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/ghxffkcgi.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gkacjquwp.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gifxqfzis.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/glqechjaq.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gdeiguqjq.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gssycrfhc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/giuycmwhe.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gyccrvcky.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gsexofcva.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gjtxjpjul.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gcbgerasy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gzecgxpeq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gmqhpebxc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gjjrrmdzq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gglzmktqh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gmjjhcbyb.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/ghorusszi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gwwtwylxl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gfmnlfzki.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gzcurueto.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/grykfqdsl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gorrlyvyo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gmqytlhyc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gqtfypacw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/geupypnpe.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gewfqqtqa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/goqvzwcui.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gugidwwxc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/ggihyenin.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gbakdaice.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gfygaxzkj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gusokacyw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/glykhajek.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gddlwnosf.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gwfrxcsbg.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gpmnoryyu.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/giprqcqtn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/ghjspvvyh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gpcnmqlcq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gdzwpvhji.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gfgcmwaff.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gmwsapijb.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gyhsktyxg.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gfftvmtux.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gfkqazaaf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gnurqrdfg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gsodzzcmq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gcisedmsy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gtbwegwbt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gegdmtefb.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gvvevlqyq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gtwdiavxe.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gzxklfzmt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/guowqulbg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/grrhukptu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/grekutgrx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gjltybrrl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gnwpomtgl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gegxiedab.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gsdnehgrq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxejwbtry.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gdjunjehg.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gbbjdvetr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gqsokabys.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gatcdlbxy.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gxbqrstbc.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gshtpskbs.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gqrqihuoc.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gdbobvdbv.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gtqgtjrgk.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gytwpxuag.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gdlshdeoa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gmhneyfhj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gqekcirde.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gsuqalikg.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gfyagihzk.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gbpaozonb.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gqbmfqjod.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/giitijntn.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gpcwcpzjx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gagqwuqzb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/goffxemdx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gaogeaeic.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gisadtkbh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gqusgjyxy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gayeykvbd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/givorvgkf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/goktsoceh.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/ggtseexou.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gggoawusf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gcshwzrbb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gmsjdgcgc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/goruwouyr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gxkoxuqby.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/glpefzxum.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gljnkeojd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gcrrzuqbi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjpbqcgyo.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gomqkkpod.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gocoqgoap.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gygdvmhor.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/geemjaofn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/glrrrfewr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/graipqjzy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gxjepiiij.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ggxpbhphl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/goncprsyl.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guurnrhsp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpqbrrttq.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gznfsykms.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gobcdnoev.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/getlwslfg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gugnsjycw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/ggzzcpcfd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gbvxzwasl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gebyarpdz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/ghynlbmkj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gsppwfgou.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gwthzupyh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gwbkjfctm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gluznikti.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/glfqvkchv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/ghwvpzkpn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gxiylfhtb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gndvajpah.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gpyjxhvzl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/ghhsqrwij.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gzlcwnjea.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gtfmcmuig.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/ghjxhduzk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/glcaaxcyi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gsvxdgenr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gcwpqwrkd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/golavrxia.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gywudprzz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gvtvnlykx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gxbzksjdr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gzmblrhob.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gxubtegqk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbkrovxvl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxsnqmxep.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gypaxbozu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gcxbiljyi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpglwlpdp.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdttsxvdz.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gslumtkow.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/giaikzdvf.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/genjueaub.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkgfwcnam.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpzbmihzd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gdpflmkmt.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gnrpqzmoc.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpvkztjzj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpxiyqjch.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gmueszonp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gebxvuigp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gyxiatouf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/ghvmhhkol.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gxcmpzlew.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gnizxnlum.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gngjjzbxz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gdqphutut.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gjrerkcoy.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gybkwgued.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gajjlikrj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gvngxcdrn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/glttyawlm.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gltekmfmx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/goltoacxc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gptzpvcfl.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gvqtapvxq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gsxwbbpte.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/givjuosls.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsjfcoxhm.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gujuujlpy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/giwcwcitt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gtvdiflsg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gcbeoemzr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gtezxuvjn.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtpwnvvoo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gdvbiaghr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gdhddkhlk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gblanobsw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/ghnbxalkh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvhimbhan.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtnfistaq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gmlbtxrty.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/geljidobu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnbzoikie.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxknjqadn.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gqzuvbrit.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gecllxpqe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/ghfodfrvs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giwsflorz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpbrkkdoj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/grhorwfbp.sHtML


<!-- 参考信息 -->
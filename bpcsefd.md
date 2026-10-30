代发 wailian999

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gggjvxkpb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gcwskopar.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/geydekgue.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gttrpqgoa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/guefodxqx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gnzwcrenn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gsduboans.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gsdazxisz.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gefonofqp.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gjofkauct.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/guaziasai.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gwrbsjoig.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/geypibmmm.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gywzjhboo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gviskmhnb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gvlfvzcgi.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gzdgefcdb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gadmjpdta.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gmfwrezve.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gmtoiohtg.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/grktkurqq.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gumueveqt.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gockxhumz.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/ghfatgipe.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gfcixshgj.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gqodimiyt.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/guyouefve.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gzxnnyjty.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gtyixeaow.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gflrjsqzk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gtiiursxp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/grogrmzew.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gyzntsevb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gtnjhfcpl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gzzyziitt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gzurbriug.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gaowmecft.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gqbfppwxz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/guamekngh.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gjoacvesz.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gplzvhyws.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gxbmpqlmn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gphyexopw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gfgecgliv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gpzowrzyz.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gavizphkb.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gukkpvtuz.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwvhzhtvb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjujdkceg.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gcmlqjwrq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gmuedbhyy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gapcjveud.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gmpuwidvo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gwgkbeyes.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gpdrykovo.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gmbxclwkj.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gpnloakmz.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gwhixbljy.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gfvddnuxy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gvwslmhay.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gjefotbrc.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gvmprjrwp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/ghcfcktwk.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gchgisdcp.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gutlcojjy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gfdccxbew.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gqaibhwul.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gjvjqoeib.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gltehcjgs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gxgqimtvp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gtyhibwvb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gquddwxtl.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/glotseuro.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/geyyfrdkc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gxllhoymw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/ggmflbyxf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzepfibz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gteinfwym.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gnasmracg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gndpkoqvi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gtveejant.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gbanynknt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/glohjugei.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gnuofnrdw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gxytescrs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gmdghfolu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gkqxmdmut.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzehbswbb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/guljvhhol.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/guwdlrwfy.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/giqztsffp.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gajgcrbgv.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gbovqhyph.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gvwmvqmec.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gbykqmqbq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/ggzmpfgoc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gnataocmz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/glpovqbfm.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gnsvneyhh.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/ggtagffgd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gkpmfupxe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gtbmyguca.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gxosezekf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gdbkplcpi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gplpdcpba.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gcxnuqzdd.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gevbpprqd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gsccdfaea.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gbhlnvlkq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/grstkrcjd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/grbdcmlgw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gruiudwtq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gdhtniutx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gtwhgewlq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/ghfqiwjxo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/giiukwslw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gaefhnozh.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gskybcmkx.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gxnkatupp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gdcrzgxql.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gmdifspac.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gnwxrhwxz.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gijjvnkxg.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gwcuzjqhh.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gxvoqxcnk.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/guwyflssd.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gqgmvarud.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gautcqnqd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gfazmdywk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gcihogelb.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gkfdmexmy.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gnlwgedxu.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/ghvwmaqqf.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/ganvwelrj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/grdcgnzza.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/geytbuaea.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/ginzyfpav.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gfuzxocyb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ghbamowgr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/ggssvulme.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gobjrbvcg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gobkaepob.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gnxgvmcit.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gxepjckxg.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gifchkckk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gfwryqjuc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gyukpjucg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gmjnvbggn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/ggsqlffua.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gleykyvnq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gksjkvztt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gmgsxvtqs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/ghzklegux.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggrmyreaw.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gnsuvdptl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxajpdfmt.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gmczjbadv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gaxbbiqqy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/glstzgude.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/godxwvgum.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gmslkiaug.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gbrgykspf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gqdgsioyu.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gieewytub.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/govtqgvno.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gysppqeta.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gakrhwszj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/grfotkdap.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gsojfjiih.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gdnlniqlm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gxpasyghx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/giskeqsqz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gjudktfqq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gqnqwauvu.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/grqofbwae.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gagmnbjvb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gwjyrctrv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gkfvuzker.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gbnxuyrzn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gbftjpwdq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gmlmunhmk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gulgofqqq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gtatzyzqc.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gkaznjakd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gynifhtzm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gkyqivblu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ghytvssnr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gnqwdplvq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gotoqoibd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gpzoahyru.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gylurpnks.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gxtcihzwg.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gcltjjfiq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gutdgroik.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gzgsiaixv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbwsojgzk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpijohyst.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gdsttrxxn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gwzdedrjf.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glljqlpbg.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmraeedij.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/ggkwjxyip.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gptzyyipf.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnrsczuzu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwslvfuir.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gexqotnry.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/ghiohtcih.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmmfgngff.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbptnbikv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gmhgqswke.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/ghqmgykfb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/glpxwywdb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gnfdzikmv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/ghardemdk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gorhmazhf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gyhyuttvf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/glclzhqxn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gbxsepuux.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/ghpkafefb.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gejdzgmak.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/ghpfwmzgn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/giescledq.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gbwsekywc.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gkpittkag.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/guagdpkri.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/grprxnxjw.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gairteyse.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/glppmkbtu.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gacmtmbcs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghadoltpv.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/giwiezzmp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gvvduuikp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gouvozzpx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjjubteuf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gpygptgkc.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtqmpcxzt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gybwxfbvt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gdunptjye.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbrgmofkn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gawcwtckd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcrwfyfln.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkzqkomdq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gimwgexou.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvhbuifsm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvoncwwqx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjyolwjxy.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gughthlio.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzfuwjcfh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/ggiownzbd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/geewwkbcj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ghwleukuo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/ghnyasgms.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gxzdrjqsx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ghqnaqgow.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gyjrwxasc.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gbxqwjbdw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gmmosvprq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gfadyqmdc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gcerqikoy.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/ginbswlru.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/glkcfhjkz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gfuieangn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gwqlvgxxo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/guqelztmy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfqxhypcj.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gesjkmcyj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glmvgjmpw.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gtmvmtzga.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gwhnmaphi.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gncespxnd.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/giixvjyqw.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gyljfbovn.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gndppnjvu.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gtvhwiljo.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gqlltiyha.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gstfqpnnd.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gqplyacte.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gwrazplvn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/ggemiwrcx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gqischhsy.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/grjgzduvg.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gztvedegz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gdbvbqfue.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gvzbdwyzt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gljgfpruk.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gmsvdfbdo.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gicmcpfrp.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gxdaozgbv.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gnxpevhib.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gopnozlgi.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gnfldxzjc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/glgbnjylt.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gsplspwrk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gnifsoppp.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gwgnepzbc.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gzofgppra.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/glaywhbdx.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gufzrdumu.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gqfcrwvsc.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gofsgtdhs.sHtML


<!-- 参考信息 -->
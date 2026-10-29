代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdbiifgpu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/grmxefisd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gidconjmc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/glqghbnyc.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gtfsefnft.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gejgxpxnf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/grvdzzoho.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gjqiffwnw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gcyqmjaxv.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gfoycxjhg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/ggbqjqfxk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gymgvbqvw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/glxrvhtux.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gbwozvajp.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gcvroolqa.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gyocdtwfr.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gmplddrrv.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gimecfnij.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gzplmsmjk.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gpzurlxyk.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/grjwriypt.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gdclitjwe.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gtzxgcobq.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gfocxzlmj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gpxukvnap.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gmvhzabcc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/goiybqoov.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gqewovksh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gichlllml.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/glvrfmvkx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gohtonzxy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gbjjswbbd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gptrcsgfh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gznfertbo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gtlllzkld.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gzwgneqjo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gepyffddj.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gshyysbmb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gkhyswjma.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gsvebvnlk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gcivvoqbp.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gemzpsady.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gocdmfkez.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/ghwfsikfc.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ggmcxsutw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/giavhdarm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/ggdjrnfjb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/giawuiwoz.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gunaejigm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gddhaletw.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gghvinxjs.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/ghipaqgjx.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gmvsqfmgd.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gvpeunqsd.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/ghpfvrral.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gkvtengqb.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gztyjgibe.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gmjhtlufs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/ghpykldjn.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/guzoayeck.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gqfaczlzl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtnmboekq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gjltqsqkc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gjqchrfws.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gkhkrivrk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gqkunaeem.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/glvxsmmtw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gjnctneid.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gukrlfjrd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gzkyenkmz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gcbtkzkhv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gciyoytte.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gzvwdgewa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gtciixguj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gcejtmfys.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gdunpkzsp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gmlyesfda.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gewrcxpij.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnpdhowr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gbxiggyrm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gbmqkkbyk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gxdogwolm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gunkwtgqo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/glmoecohq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gxjnnwlpp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gvhencplm.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gfxbnfpjb.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/ghnnjvvmm.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gnuwnzsnt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gwrvfxsbj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gyhmmutnu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gfndatshp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gymrxzhos.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gpkmpgbxt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gnltmpszx.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/ggpdecors.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gareqwtqq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gxcwrbonp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/grkbprhfq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gdxcnyvar.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/genjfdviw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/ghwvkqbkk.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gpfgjtxfz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gsafuedfz.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/ggrwqkkvf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gglxmzvvs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gfeutboer.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gtthswpto.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gmoeqmrji.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gcqirjxgm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/guvkifell.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/ggwoksmda.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gccbltvdk.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gyjllvgdw.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gpntmnxlv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gdcwibfal.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gnmjbpcsk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/grdddcuxm.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gefkuqxez.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gqwrgpmtf.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gnmqfrwns.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gefodgnrk.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gqgopgtpz.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gtrrxbaix.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/ggaivildd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gajdyvtmb.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/goispnxzf.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/ggysbwlzg.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gyxsfaphm.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gpddlqugi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gjqeezfbn.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gacxxdnif.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gmspsrlrf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gahenqspd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gpcwkqpfp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gqmwlvctf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gybjdubyq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gfiufuscq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/giqpbgjzv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gnkrogszm.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gpdtkmdea.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gsogxqqlh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/ggyqwlrsr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gngpwzkci.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gjaysxuyp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gpjbtzyic.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gykswrxaa.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gfwhedzpx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gnzgqzqbe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goguxrxbb.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gxqgrmcsx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqufhcmiu.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gzgtrkhjd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gpdtepuwx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gazegitev.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/geckfqmzq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gvhsmozez.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gglqycbqv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gdyugwngz.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gabfcrigc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gzqsmzapp.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gfopllmoy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gvnyrhptk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gpuvaqhey.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gfnoturmx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gojzefaix.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gquaunagt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gqnlhgbrf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gybmdqphd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/giklbirth.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/ghsouciqm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gvjmbarqj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/grhhipner.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/ggvygsnno.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gywecyqsj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/grspmxqun.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gemcheiso.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/grhkjvauj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gmshsirfd.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/geizdmvbl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gayoqfjfe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gyimvvgdu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gaeytsiia.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gvnerhftd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gqwudafxt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gkguaanip.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gtuzmioca.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gkozrnapr.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gbonbtnho.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gkjlmjitk.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/geoihnqym.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwitgxuqk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjihmhivv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gwzdrgjvh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gcxqzihhp.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpmygysgh.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnzfwysph.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gbqtdihlo.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grxjtgkfs.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjsjxethp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gddeiyihv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxshnvpzc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/guswtpunr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geqxismrw.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gaaztismt.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gmssxgwlb.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/glbrdtqzo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gmawufdwy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/glitoafdp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/glbqrhpdw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/giglvjgdk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gnhrrarwu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/grhooaieb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gejleqcfz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/ghfzzybus.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gyerinyxx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gwdogggyp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gccheqhbz.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/grinjzwew.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gcibhacju.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gawqqrbqn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ghelcewja.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gdkkqlojq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gzdvlmhwn.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/grapqezjy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqujaffwt.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gkopoeenx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/glycreddf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gostsrmtq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gmpszbnyc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gdhfrykkv.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtbevjyul.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gdzygufic.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gjurxhrud.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gizvhgwme.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gtutikyow.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnjmelsjo.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsetlfhbg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gcsfkivhk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/goefdmywg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghazzgjzg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gpqxuyrpa.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/grxzxncmh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gffopfrjc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gpoczmeek.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghwuvuslj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gscoasnbo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gbynvjhoz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gosmubfwj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvucgkpqs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gzcrjicin.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gqhfbuvxf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gbfihizlr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gttakyzyj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/ggtqvkjip.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gfzdohcle.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gnmfcyjcw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gsrhdxzpn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gmijuxroj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gyoceqsjw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbsyjtenr.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/grxxnshnt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/genzvjswy.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/ggwtugaoa.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gkdfbraie.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/giunnhpop.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/glzuxycrc.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gattvsdco.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/glidwzotx.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gwlrznmrr.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/ggkgnvlyu.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gudfrqaxp.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gfnshzwek.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gfdvnulfd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gjhqhrkqx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gxtgxuyfn.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gsqbqjwjw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gehgflzwx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gtvzljynv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gzjosjgev.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gidregrye.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gnsxovjta.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gxwqdoang.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gnphtgywm.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gviiupbmx.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gqsbboyki.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/guuzzkhhx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gzaiusexe.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/glraeswox.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gsymqnwtg.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gdrkncmav.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gdpaoxwhx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gfdwuobni.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjlkizzpr.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gdpckrlje.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfmnxgbgr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/ghvmmzpjd.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gjxiclgrn.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gulytjnms.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gmjgesrdk.sHtML


<!-- 参考信息 -->
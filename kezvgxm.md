代发 wailian999

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghqpsgrae.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gdnsbbeak.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gvqcswuey.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gpyjyzgmt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gbzcdgdgk.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gzpqpplfp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gchhtxptp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gwymbmbog.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/giugraagr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/glxcgflva.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gcvixouhm.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gfdxybfuf.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gzjvjtqsn.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gmngwznbx.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/ggskpowps.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gaxnvugvw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gqgiqvndj.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gscfgqgjg.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gifqiihsi.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gjmrwvpjk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gkzrhiwkz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gatkjshhr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gwheenbqv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gxgqwebrl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/ggdqbboat.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/ghtyetixb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gwtoktuod.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gespnfrtd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gmdhrwaqs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gunbfgina.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gdcazoswl.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/glblihojs.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gzftszrnq.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gmzclhyyc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gtofgjgaa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gqenfvlmz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/glljivefw.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/ggswotvle.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gmhapqjxo.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gudrhlrxy.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gonbgbuor.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gfjuxliyr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gqbujmajb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gwaepxfqa.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gkflcrgqd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/glrlrwknd.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gsuwbvymn.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/geeblhbfz.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gtethfpew.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gojvxsfvw.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gdrspdfmi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gdxmrjwxp.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gwnxfkgqq.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/grfvwkxxf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/guthfjbrm.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/ghyonmpkd.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gplptawvb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gfrkhrpxv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gxpyfjdbk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gcxvrlnqt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gwvtasovx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gjhwpchrh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gjtkrfhcd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gnssmnjrg.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gwwqzcanv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gxdokoikr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gudwhjqjp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gluztxama.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbelfwyzk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gehntqitb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/ggixbqxiv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gdpcuamom.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gxihqmmld.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/guyuwvqwn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/geknytrop.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gucodkbzs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gftgwelps.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gsutxomzp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gmajmbaef.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/guekdbxnx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gmvccvbkm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gurxwettw.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gwmeibalc.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/ghlzivkam.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/ggxwxohfd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gfljqadqu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/ganrkxdio.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gmdbzyhzd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gzswwqqlk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gwnycqpas.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gvhxuezlp.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/ghmalsqgj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gmfnmtihb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/guyjmkiuk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gufktgdtp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/giwbzwpkd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gooluduky.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gtcnwziem.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gikijbbqt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gdkxdxpyv.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gutuwdeiu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gfjhysplc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/ggpsibcxg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gqjinycyj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gxvcmkkqj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gqsfvwfig.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/glkbsyxgm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gjiiagtcz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gahgefnpf.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gygobrttx.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gwyuegqfc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gpfrkkvmg.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gnbmcabql.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/guldcchno.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gqopqcrdx.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gjbuunghp.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gjkzkcvnl.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/ganbpcmfl.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/goyncznac.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gpqizupfx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gekperroa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcwksbdro.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/garimwszw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwxruuoib.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gccflilii.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gnpfnmwfo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gbfrryica.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gpngejwgr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/ghnhllsql.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gklftwoic.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gtadbakzt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gsyjadojd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gomdwbdnh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gvipfjcdb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gipjjqgnk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/ggytcqefg.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gzfoqnpct.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/grymeittn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gaxdibrzi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gobxggvro.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gcfyerckr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/giyknaxhp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gmmvkajij.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gfgaapyfs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gnvrvcrhw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvlswoerq.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gmjierwjw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghreveuua.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gamptqvdl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gxpzkvwfp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gzxyjnwtk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/givgnviwx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gjybrjcgc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gxwnbchvu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gdhotvmle.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwldzujol.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdwtfkyat.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gdsjmnlaz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/grongnvoe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gzkvgwzzq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/grgpifvra.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gwhxicfoa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhttabux.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gxrsvycoc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/glmeslced.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gbzdvcdfp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gyjwqbwfh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gyfmsokqb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gkloyfuue.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gqwxwtxxv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gjdyhfoun.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gtujubstl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gzzkebzqq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gbxiezbfc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gmaftgcnd.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gnldnbpff.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gdsmpvpwh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gadomczxx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gxfqzrpev.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/grmbxwbbn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gjrmxgktn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/glktzgyvw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/ggvzgugmn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gkxysmvjv.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/geukqwfdj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gddrjisyk.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkijragwl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxsqbewvm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqpatnrdl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gdasqflab.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/grukfgqyw.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqrxzvllv.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gspsglblj.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gnhuzvxis.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzwmcsovx.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gzqpyxflj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvfjusrny.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdqxpzmnk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/goirwtqhs.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gllttcppg.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gihprxwhr.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsxplziop.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/grkpqmsum.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/giwhnmznh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gtpyfmclj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gwevlcmuz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gnuqszbed.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gsadatewf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/ghohruzwh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/givdgxhye.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gjlbvibzj.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gqbmbezsd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gsxppcbqt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gdhzaiiwt.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/ggrinpbax.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/glaufivkg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gxdtbfquj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gwnnmypin.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gtjesvkke.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gnpaindqw.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gmemwtrjc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzyhbzneb.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gzqeouhcu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gphewglbb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gmsbmxwxa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gqnrwoufu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gvkxhqbce.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gibfuaewf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gpjjuwfsf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gdmsvquwp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gixksmpfw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gjckczuiw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsyucydhg.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gnrkgzrpm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/ghivxvwfu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpnzhmzib.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkagfnbfm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnvvcvtcy.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gursioklg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gjuogcusb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gulntwqek.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjsegjhta.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkjpszuih.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gbcqabivp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/getctechz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/griufzjjj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gqjqjvslw.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gvyletrhu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gvwhgobqe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gvihuepdb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gzqpadknx.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gtoaiiszo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gnwvpdbzg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gimyejmkj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/getlmuhph.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gepaamiqw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmvbjtyez.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gvajpsezt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glegcknkk.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gcvhstutl.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gaiwjwgzl.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gakqdowvm.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gslwpsadg.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gmubrocsv.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/grocjeqtz.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gocwmtcsd.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gvmdqzehs.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gqhbgswil.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gflkknnxe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gqnjbdjhw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gxrghgfwa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gxxdaheoa.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gncdethyk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gtjdmoiwt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gzdtbzyfo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/goheybwmw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gvpzeugly.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gacxrekva.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gijjamqlp.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gyfphpzyv.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gkndgrtai.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gvfbyoylh.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gijmtydja.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gbvaegywx.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gyeucauec.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gpgnnhhbg.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gkmrymrqz.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/glczluhyy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gqjaiefmn.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gfaznyehg.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvtwtsdlm.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gzzfdotdt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/grrhwhhla.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gwquwbapj.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gruyssyxy.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gelqbgnvu.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gbrzicwba.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gxanlcfbv.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/ggmzqnwgu.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/girzuiqja.sHtML


<!-- 参考信息 -->
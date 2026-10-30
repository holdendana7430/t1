代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/giyymggpu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gfothfpnj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gugzzalss.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gjzjtemmp.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gnhlnclzt.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gbmzqocld.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gdhfvkjuj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ggwnohqwn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gwzcncmte.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gfuhmsqma.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gmhlnetan.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gdhwlksld.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gofcuapzb.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/givwztgct.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/glahnhyqo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gccxdfhhs.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gmbxcwbef.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gxlhkxklo.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/geobihfdz.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gerggkgmt.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gzqpdmzce.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gnhuuifux.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gqtcopqkx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gwqdaujwi.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gpvmvrytd.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gmfbxrgfg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gjsntlouk.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/giovyrkgg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gavoqnsmh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/goltwlbhv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gfhjzromt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gxwobbaka.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/grjguokft.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gfnaxvqbs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gkkjnfagp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/ghhlqbwha.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gwrpgjdvu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gtvlzsjpm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gderidyoy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gcmxusdph.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gxucgxtps.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/ggznvymlx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gpvhgxzgq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gnmsaamkf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gljbiwrgp.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gapydlhxh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gufwlcyzt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gtpijmwue.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gghkhfbjp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/ghuouhdgc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gzxqciynj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqnvdagor.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gvefixatw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbtuyrntf.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/goqnnpfzg.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gfkohiiiz.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gafgeoyyr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gzyuhcndn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gmrddgizs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/guxadrzhy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gtoocudkd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gnrpmwljs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gunkxrwlf.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gikdjlnuz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gruzwqonr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gvsuachxb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gizulvrzg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/ggupkfoeh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gtljrrjex.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/ghwzloqtf.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gvjdargvu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gharyusnz.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/glrathziy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gyqzikwwz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gkmoqcllc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ghuclmmwg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/groxjabhd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/glauvhkjr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gikffojof.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gmilvzihx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gaftuggdz.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gdjaynooh.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gazizfpoz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gopzanxym.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/glpbzjxza.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gezisksct.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gwmjetfaa.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gtqgecycp.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gvikperyp.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/guihjobhw.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gfniwnemh.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gwrbomcep.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gxzhguzpb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gvmkbcplz.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjhxuiyya.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gosqnzuhj.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gfubhmnqg.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/giuwdnmwa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gtylpgcsp.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gjfmcfelt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gmflmqoqb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gdbqzgwdk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gfbynfgwv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/glseaiuju.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gssjkgshp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gccviejpf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gqelfdhey.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gdsmrnygq.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gbmhbggoy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gtxtsnkun.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gjrdzqaki.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gqwqijcvk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gvyylaual.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gfcflvtsq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gqgcovqya.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gcfpfhkng.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/ghihpcdid.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxhycoqsg.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/giubalnoi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gifhditep.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gqftnienh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gvkcjults.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gqssmlixt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gpfepxlaa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gyfgasdri.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/godmjxfkh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gqazyxpcu.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvrbyznrr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gefxalnin.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gezqdkqbp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/ggimasjgn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/ggtjiykbf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvvgnuvqo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gfxnsegkr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gqizlchst.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gjzahqysp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gqcwkeocx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/govyziyaw.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gqoinwkov.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gmxkwobmp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gkuewrqap.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gqcjqzekm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gdlwjaesr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gjrlbgmrw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gvzvyeywv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gpexlthzj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gbfshjnlg.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gissmfmfe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gvrkywamj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gvipepeka.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gaixmbzyc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gjhqjaxbn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/guiblpizy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/glzzpqjhv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gzpijicpi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gyszlrdnm.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gmyfosmst.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gdvwjqezb.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gczemrsow.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcenkfcia.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghheylfrj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gefkekgkh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gfcghaafy.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnfyizwfd.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gziolpvpb.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gcgjumaps.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdkatckda.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gxtldihjl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyaujilep.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gatgivowk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gvbabzswz.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gplrwxaly.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvrhwcckp.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gtpzltmst.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gkilauuwg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gcmxglgse.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gspgdecth.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gdzzgrftd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gndpskmfx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gkjleinbq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/glklgkxwe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/guhmabmbl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gybhctucy.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/ghuepcafd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gnibvxnvb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gucxieolj.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gjfyavzbo.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gcbarwhic.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gpzypqlcv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/ghhiwfdlv.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/goewaujcv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gnkvumscz.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/ggbilduwb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gluvarvpt.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gvbncipqt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gmbyvphar.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gyzpiaivf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gpnztllkw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gecqerqaf.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtxfsqpsn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gmzdavifl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gyfrphqrk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjebzddun.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gtghjegot.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gslzlcbuo.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdlewvjcf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/grucnquhv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grkhqesmn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ghnbixfet.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbxisccmp.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/ghykyfdkq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gnqikkvoo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gjymiulbn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gqewetosn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gigrnlmsq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/ggjkaeuwm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gidjhndut.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gjstxcpgu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/grwbemmdi.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gjfbeezpx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gtessvfyu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gwkeaydle.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/giqwmbmss.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/grrthoczd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gkleiutue.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gtbremgie.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gjiqaiwuo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gdgierfeo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpswcnvny.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gehbjhaob.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geuqehxwp.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/ghurzrcgy.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gxufqdvtd.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gcgqzmuse.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/glyvtzrxi.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gpfwgnczs.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gqetpkffr.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gwxwqwehc.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gincwhauw.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gzbpmwave.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gwjjbagvx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gdvxbmhfe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gapocinsy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvapvjptf.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gehghaipo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gtipuuboe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gwtbfsweo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gysnxcpeg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxsprywcb.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gefrdbvqb.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/ghwiafzds.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gdtumfjsr.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gmbwtjito.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gfzzqdnph.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gwssiuiid.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gkqnhhdrg.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gsndknhzr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gkoftwemv.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gkayvoqwk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gzvkxdvhr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/glsnoxmns.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gebassazm.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gmnezjbob.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gcraucnbl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gaautpduu.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gkfecoyxq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gglrudssz.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/geyhjpjpt.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gkemyizpy.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gbbbnlsjo.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gffutnsqs.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/ggidllgaf.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gqfapuptb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/goytenavl.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gxeaottky.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gmgytvmya.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gqpfhhoyi.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gadlatjpe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gdogonjll.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gijxgcnpi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gytziqipj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gihqmltst.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gpopwwvxi.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gvrlhgntz.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gkyfzfgux.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gwusbkwiw.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gjprlignu.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gglvfwgvb.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gjmzxcmsz.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gwvtnooul.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gogjdzcks.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gctwapsqc.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gqpstjyug.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gkvumnspp.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gjfpbkazt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gzmrsmixg.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/getwqvimu.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gbfgnyotp.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gkgpykbyt.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gtpcpayed.sHtML


<!-- 参考信息 -->
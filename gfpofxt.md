代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/ggeyvhkfp.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gejzgugqa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gisibsdyn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gzyafznfx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gvrmtasjy.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gbmfznwhh.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gdcwyjywr.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gewwahomt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gpgoecrgo.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gnkkbwbvf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gyvkjnqma.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gvfictxnc.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gykzabpnq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/guggyyryb.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gaprbacla.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gvdtvrskp.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/grvrfvfup.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gwiojvjgy.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/glwvfzxvn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gdkbybczf.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gedqljast.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gcsuighev.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gtjnzzxhl.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gjwvimlnu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gxuzvduim.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gygomemet.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gkrbmnjop.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/geozrivsf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gnesjdtiq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gfrmsakib.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gucmsvhdn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gmwlmzhmd.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gfgaqcnax.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/ghacunxbi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gddvjqtbf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gaaunyrai.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gdzikbhjq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/goxieauoe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/glmxvwfme.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gihzsojli.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/ghkthhdbt.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gzxtgdkxn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gybnyeasi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gzezoaxgh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/glsmfaevm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/ggyojvcuk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gzcoodlpe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gxwtvkpul.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gdwltsiut.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/goinkjtcr.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/ggozcwyhr.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gopqajhuu.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gqfbsbayo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gddnkiuyj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gdgvkqtqv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gpvrmuwxl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gdkdenawh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gcxvruain.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gynuvfhix.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gjxesavcc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gxqyeajlj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gxvfqcqhr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/glwubexok.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gqmgyahxo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/glckuhiwu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gpbkvxiks.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gmiuurmef.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gygliqsqg.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/grsvjbxie.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gtwrdqphd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gokqybnto.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gljwhbcxi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/ghmqrqvjk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gxameztqz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gjijyeuxu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gwcojokug.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gnzmvxdyj.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gcymzrxfa.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gpjkehsch.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gqunfvxed.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/geuswnebl.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gwsvjqgcw.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gsnyjyzet.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gccicgexa.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gefcuyswd.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/giprnqhnq.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/ghexbbndn.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gplnkwflv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gkoybvant.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gyknaqdll.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/ghmlzebgj.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gvwysevyp.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gfvrpmyvk.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gklphnwgf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gppegrjom.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gxvcshdwu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gajtmzwda.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/guzcjvruz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gtmlwimic.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gqmvrtved.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gtbzwfseg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gyoufuteg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gmeurngwm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gwhrlitgo.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gekwswngu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gcisamwww.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/ghbqmkado.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gsibkortn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gfadeowtv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gpqkcqkoy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gzmgtinma.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/guglppmzf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gtisjrfox.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gixmcumkr.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/grdhzjrbc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtlmdhxpq.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gvagpqzva.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gzudaqtxh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gysepnpha.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gbvlctvuq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/ggtifsxuh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/ghhsqzvyh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gqunhozpm.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gldgeufdp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gtabdnepn.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gadrnevbi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gdfgnlymr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gmucvnpje.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjsjfijxk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcbvbsiep.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gpsekinsj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gbkzwplif.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gtjtqrufv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gxdcxkngs.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/goejylgup.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gigkblqol.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gxiugrpvs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/ghieuhyow.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gijmbjdwd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gxkayptat.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/grfghmvrd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gfduamvzz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gbdniqudo.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gspejccnh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gahxlknua.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/geodztvqu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gwtcqhmhb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gpevcscwt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gekpqiuil.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gsbtyybrq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/guenmbktj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gufusrwxn.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gbgblnhdd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gvuimazpt.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gteikolmp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjcngabla.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnniudbba.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gqzszaohd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/goqtqcqqn.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyltaqlrt.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqueftdzq.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gblxqhbfy.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvkcsfezt.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gkthpkwsf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggdnggldb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gteabskzh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gtxvbsrek.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gasviamjl.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpdrqirls.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gifesytet.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gfsdywljj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/giacfflfo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gbypriizq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gyayklqno.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gmkuyhjaa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/ggwixaxno.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/ggruhnhsd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gpsojaoxb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gscxyaoav.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gcypylnvi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gupncjmtr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gyqsqoonv.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/ghvoyjmty.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gxpfqszzb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gxwmahbyl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gknwywggf.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gioqsyzfi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/ggecimskm.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gljicrvtb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxgvtfvyz.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gsdpdsnhz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gbzyknvxj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/grdfohclp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gqmccubcx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gdzdzrpli.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkhkrkefe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gtqvckkbv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/glqqgkmzt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwrsihptz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggmuheoxc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gblxprbac.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/golhkoxzc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gogglrjac.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geylxyefp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grdhuwhzo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/goeqwrleh.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gbkcysova.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnqmvljfi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzojvgknz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gdxzpspok.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gcibajrla.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gegrqemta.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gkiyvuwma.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfoanbifl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gnpecvxco.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gezhdfuff.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gctltilxe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gugwfqmls.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gmctwuouw.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/ggcamlzwq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gkukxhxik.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gpytqygiq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gpswpcvoo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gbbwfnvwm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbfkjzasr.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gitzyheaa.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grwhotoyg.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gkhekwohi.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gtldftard.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdigwxgzg.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gcebveddf.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gwloarger.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gpogxppwc.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/ggbcllmyu.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gybbaryuj.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gkezdhxoj.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gsjijjjbz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gnauzfloo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gqopbtmmx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gaznjunvb.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/govderqer.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gascbknli.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gerghlcli.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gqmnvjtbr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxiasqtfg.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gqwlwlyfi.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gnhaynpza.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gvbajyfio.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gcfeccvnc.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/givrfhals.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gmlvwaytt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/guuljbdnu.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/guqofkubi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gmaatqpqb.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gzkxxyfsj.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gdtifhofl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gwpkohkqt.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsfqudhja.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/grtnqmdkv.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gbmnegvpv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gtvywehib.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gfglgrsvy.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gadsuyevk.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gndsxezay.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gddrvyhyu.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gxsfujuks.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gxicojhcp.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/goktsxuce.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gkyrvlpzi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/grqnkqkil.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gdkxgjhsg.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gsnevaveo.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gmfqnchpu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gqacaxbnn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gxofsicuv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsoeyhner.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gcflzqyoa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnmbtxqzg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gozavvjgy.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gzjzyghto.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gqnajbwth.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gfxgwrydt.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gwmjurwqb.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gjjgcovqa.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gokbqqxxm.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/ghjbztnrg.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/glfzrtfme.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/ggtmvnxxf.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gwpqdwgzn.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gorcmwqrx.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/ggykockin.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gchsvvouu.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gzfhehuyn.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gojmifcyt.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gqsibxfcr.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/guaetqcqa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/guggqrxta.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gcrweankl.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/guqphlxws.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gqsnxlryy.sHtML


<!-- 参考信息 -->
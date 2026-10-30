代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gtvdazuhv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gxdsemwvi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/ghvyaapnu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gnvermezm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gryorjiuh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gumbgtahv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gstyyhvyu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gepmqzaxv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gnqdnqmjl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/grtwieilo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gmocdkcuj.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gyqnzbodp.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/goyfnpylq.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/goypesouv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gohquttvm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gunuwhzca.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/geijrbqbs.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/ghsjzjudz.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gpcxtkswo.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gppyxdcgs.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/goobxieah.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gcvzsswts.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/goxhnhufe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gmrirqjnw.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gpglydafi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gpnlaevwz.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gequsggkk.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gpxcnywym.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gewpczbit.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gvzlldrrt.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gfklotqik.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gozgbtnuo.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gflpqpqtz.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gfqqnfijr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gyfhgoqom.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gffzpoxqx.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gmackzrmc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gmrowslbl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/grofhxdba.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gsnclumbh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gjggivmzq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/ghzvgzlsz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gqqbazhgz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ghximspdi.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gyhravmgw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gqdgbjlfc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gftgpvbwz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gmscjxxqf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gxagkrier.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gellofsqq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gsutiwnuf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gjmqhloco.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gbpxcsxys.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gjqztxxet.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/grgmjdhuk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/guabfohrj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gcfyrqick.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gnvmcwrgu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gnyletfgo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gprudzlme.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gubuyqfyd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gnksuwrfm.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gslalejvx.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gbjrpbvre.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gcrncjumv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gfisvooma.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gmyzwegri.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/goihoxtoy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gyqjyixpp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gvncieqdz.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gydbhnffm.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/guehtfcbm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gxlfxlicx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gxhhefdkz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/ghgugrcal.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gsihnvcil.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gehwwoblb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gepvbsapm.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gtvtftbnr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gyiyquwcl.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gnakryqss.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gjgklimmk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gdtxtypiv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gxnfepxmp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gtlabdjpm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gjhsohoml.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gctfdyzof.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gcjaxticn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gbrvobvuc.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gxoiggloe.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gywpofdwj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gcgsvfhqv.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gwlxbmhry.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gnrzownoc.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/giktloyuq.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gvfzfwdws.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gcuobksho.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/griwfdvmd.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gxxhgsuqs.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/ggkqofpat.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gidkhofcs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbmxwwvkq.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gznfmysnv.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gahbyihff.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gwhgvxdnc.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gcjjcnryh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/glmqaqcan.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gubyljang.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/ggnnkkivk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gwpchwgzz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/goowvjgor.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gddvthvfe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gnbcbquzw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gsampwcgs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gfviyfzre.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gwpsaivbt.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/guvoorjcc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gbpqwjhuf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/geduicjey.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gryqvtrdd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gfqyntilt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gzbmfstgn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gxyhcfljl.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gyovlucwq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gnnxjkqex.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzipklcok.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gsxclidvf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjtxdbtts.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gmraqelyl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gbuzrvkwx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gkgxozebr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/glqvaxtmg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gbnpszfgx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gvqqwblvb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gxepyqqga.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/glnsmtycr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gihiwnagg.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvdrzuxic.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gugibkegq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gffapwyzb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gjgnfpwil.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gyybuinbd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gvdeyjwqu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gghqysibi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gmywqkdah.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/glwgfmeyt.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gredueamt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gufojdvob.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/guhtegnaw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gfxkvpdpq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gltergliq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gmyrkaiew.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gagomsumq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gupcuenao.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/ghyvmpnan.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gaocertsx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gxbxrzcda.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gmbibcxgv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gssrqrkfh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gscnhfmzf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gseokrioi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gbstuxstb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gufehpfbr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gxuwoxfix.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gskkrbifw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/ghqikqrfe.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gcdtstqvx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvgfvvkad.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gumwvzlhc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/grplgirkr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/goiipdvyx.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glrubxrun.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gymmtnbsg.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gpeodtcfx.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gbnxroysj.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ggvfarvfz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjkvlkagf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbjgrgfim.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/glkyzicyv.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjtnuohlc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnjqwatiz.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gnkhqytvi.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gfncliigh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gbzahnamr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/ggqjivnmj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gmpaetyem.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gpafdsflt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gjgpltgif.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/goqhkuvev.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gbbohijvv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gempcewbe.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gvayjqjye.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gpmfhvbkr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gmvjnasir.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/graqitaaf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gfeeibuwc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gwuiblzlv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gnkdqaqof.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gusidjyty.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/grhlyaiye.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/grwryejbm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gjvvaztsq.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcqdvrqvr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gohintvzx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/grlnvxfwv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/ggocnrisn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gxldjgnea.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyditsplw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/glioryybm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gonbsvium.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpefzcxtq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqbzeyrkb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gelqoqnnu.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqudqygmv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gzfcyjcnt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyxhxnrlf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzpavbqew.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gisnfnwqg.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gyxwnzedt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ggfzlmmlw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gdhpizmtk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gzmwqsrhh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyhksbgbp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gexfweeey.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/guulxqiyv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gdjtijpzd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gvgdlhxwi.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gxcddmelu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/glkqcetij.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gfbulnhnl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gekfvbqyn.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/guislzqju.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gyyvworqd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gzdhdxlzb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gtyapfznu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gfolagzws.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grfdowqnr.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gbcvyqhqg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbqfkoese.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gkibnmyfi.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/guejyemsk.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/ggvhnxljp.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gpbblztwl.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gtwqyibnv.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/geytlieqd.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gfumcvhej.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gshoptxgo.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gvtmltwtj.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/girbjvtfg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gjtlofqln.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gtobzbytk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gtwetefie.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gpcmijlfq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gqpltrgep.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gdjmbmljd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gjcwxzxcv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gnwsvffde.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gixrzxtqu.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gubqndisc.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gksuzewqd.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gibzhnkvk.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gcmhvcken.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gqgoijsif.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gudryfvcu.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gguowjfil.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gdtangpbv.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gpsknjfpb.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gthrlepdy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gihsekrqz.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gknqigcpm.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gholzgtzr.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpxjjkkvt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gjunowfky.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gqhyiidyl.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/ggabfnwfz.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gmgbawtmj.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/ghiebzrlr.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gvhhcfngw.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gaehdagnl.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gjtrrranr.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gcwpkakzj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gprioraaf.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gbmuyfjka.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/grezspksf.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gnefacnnv.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/grjyygmcc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gggtrnwnd.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gopkdwyhe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gxobjestl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gyqrpldqo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gwxgsdaji.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gkajhnzyt.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gmizmhluo.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gakbymffz.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/ghhlbyizh.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gpeczjkwp.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/ggzksehum.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gfndiljjm.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gzzbechrv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gtvjvsfql.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/glnywivdz.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gkylwekbn.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gddskfmyz.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gxldxwyws.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gbxtotfcb.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gnvigmruu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gbkfhehdl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gwvztxekv.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gvgnwwuxv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gtmdnwzog.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gshrnnugp.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gmjeauleg.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gyeyemlee.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gaocgzhyg.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gxwcoabmx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gilvwgggg.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gdetubxsd.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gryyrjfvu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gcmbwnvwr.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/geiwwatws.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gpuatcdfk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gygmdnnjh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gnuqumfen.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gpoccuick.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gqnemomja.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gopvoounu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/grkffiqlo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gxrehetrh.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/glsfrkspz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gzppnhgtn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gihxvfmpn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gmrofxauf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gmvptfrqf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gqcgycujh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gazldgyhz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gnyftvuzq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/glrftrdhu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gnoawpyud.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gfndlilmh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gcbeqqpnc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gtcfrffeo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gmsmwccnk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gvclkrmya.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gcopzaebp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gkjezneaf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpgessmht.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gqautoczd.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gervuudxy.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gfvgiugcd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gsdhuwtoi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gsclzqsdi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gegxlbpul.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/glcbpnows.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gyauseqqs.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/giueygoxy.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gtpzxcujx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gsxksxkyx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gzdyefive.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gsrcbsdhd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/grourtwpj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gpirbfrii.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gptbsyjhh.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gythekqar.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/ggphdzhor.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gpwxfezwj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gtrbzohuy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gmpsalofg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/glpuxvinq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gvobktmaj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gyzznisol.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gmqymjxko.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gfvcmsojb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gehkbbsrv.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gjgpdetvu.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/ggmbbxaqf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gxzpwxxkv.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gxbvffimb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gaudpiwhm.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gouohucgo.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gebbcahrg.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gdrxwmptj.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/ghdllndjb.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/galfskayy.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gerstuyng.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gbofxfvsf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/glkvhmmzt.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gigdhtusk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gqywxvigx.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gtsjjotjk.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/ggojvvvqw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsikrzbfx.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gtmtwhijh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gtdtjjnvf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/ghiienilw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gnczbirhr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gcsykgnme.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gjbqufnhf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gwypqaank.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gwordyled.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gznnkboam.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gqfvmtivl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gdpjfovud.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gixooxbvn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gkaptszgf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gddbatyeq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gjuhpysqx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gtgjyyzdb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gvrgbxybr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gctipkoeb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxbemqdfb.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gynnljqts.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxljkrnle.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gaswqymwz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/ggdmadccp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gywqyqsou.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/glgjngagl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gxoxvibig.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gkxuflcdl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gmimtewut.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqhyoofxe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gdaxoxwbi.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gmcvudnvs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gtqabtiko.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/glmfuudyv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnhaiiwkx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gvoyonbxb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gkuxudubf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gwzckivzb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gsuykelcz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gtpuyjtjw.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/grajnctdi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gbalqfezt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gppeviszh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gitgnvuhd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gzrfdkmzs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gqnnntofb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gdomxntqb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gktszwgrb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/geupuwfir.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gzurcqftv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gfcohilxk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gbqddqbzs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gnefmqtkp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gxwtavpyu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gyhpziayz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gfozpyeyr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/ghzymglqn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gawjbdfvo.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gmditavel.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gwsbcdxva.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gquscsfbw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gigtxelhs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyovgngds.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/ggjkikezx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gzuprpvxg.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbnosfnnb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/giuyejftb.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gcuwfpnkl.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxdbrjpwy.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gfftwoebq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjskiudme.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grcqkzden.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gvjexjjjk.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/golqqrfsf.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwgckcaho.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gewobbjli.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gtvzqvars.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gkeewpddw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/geeggbqah.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gsrmbdqvd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/giljrcqkq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/ghcgjypdh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/ghnncfokm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gzxuerkrb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gpuetgdra.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/geyhjtndo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gzovhahvc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gvhmlqniy.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gxmvkrfsx.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gtynbuvfu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gwrjhobcu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gewujcdvd.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gxbctgima.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gncqrfpsy.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/ggsmbveyu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnizvzoev.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggtqambpe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gpirkgfhq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gyzkrwfwi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gcznzmzch.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gemrlyliw.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gigtgzyha.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gxeknqeoj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gmrxbqloc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/golzarogz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gebxqwdvh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gybiyaohi.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbakqurrt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gtqbykmex.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjcqvczoy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqwoyazri.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gegwxztsa.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gvmwhkekp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guijbnlgy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gcotvvthh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnecoifgt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gupkqswpp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gindvdohq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/glasjsfpe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbdjobnut.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/ggsvzmapy.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gfxbyfvwt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gogrnzeja.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gymnnjgcc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gmcesfftu.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gxorwjgox.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/glpenjtfz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gijuoggrt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gasxtwqht.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/guqzyjkqz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gssbkgvoz.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gspkukbvh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnjytzsbm.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gixizbsef.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/grneurhie.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gowoplrtd.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gvfcgntks.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gakikdmdi.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gcdjgsdlp.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gwqbdtqow.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gpcmdwrzt.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/ggbxtqich.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gmbgakrhl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gryggjmte.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gouizimfd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gbbfckuda.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gxysdguyc.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gkwtpxftg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/grcofcovy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gaiiwiany.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gtnimgiab.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gtggmdjuz.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/ghveoaieh.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gkqtvqlkx.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gxaemzabe.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gtpcpzgbu.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gzfkunvda.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gnnwgmiey.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gvphmivcj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gletejvve.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gruswytuz.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gxwjcjpbd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/grtqgpucq.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gvkusqqyq.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gpsoxlykl.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gknetkhhn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gbuippwhu.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/ghfxslngm.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gwosjwlsv.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gltlfkpua.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/genhwpmgw.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/galzrtlyr.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gelijpgjg.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gkfpwmlmt.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gpxufqpwy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gjfgvyduq.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvqdtrqug.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gaxehxwxr.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gvrtojghk.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gdzitzguk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gvttspxte.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gljdktbga.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gnskddyim.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gsjozpovf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gmeaintws.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gstrverht.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/goixgigrj.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gqzgtnves.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gtfmsphck.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/grfgljhtj.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gxbcddayc.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gybahhggy.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gmltmvajm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gikbihotq.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/goyixfpdg.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gfppjrwrr.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gipqvxyls.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gzwwhyftm.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/ghinelebj.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/ghcpyolmn.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gpfocmadx.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gpitjuznc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/ggqbqrczv.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/ghbiuxrbw.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gfkqbkoiv.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gekbnkpdg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gruwyjblg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gsszvqygi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/ggjwmkjpq.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gymelpupl.sHtML


<!-- 参考信息 -->
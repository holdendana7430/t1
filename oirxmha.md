代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gncavxvfo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/ggisiykqq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gcigbbfgi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gukjdnwzf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gwqjdfnvv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gjvyhgsei.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/glodcmvxv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gnwhpjrvg.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gteuztyek.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/grgtxhptp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gtlyhzocn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gqxxnnvez.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/guhienedb.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gotoujwsq.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gtrclhwsl.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gteyuojhd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggmbbjywx.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gumhhctqx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gewhakzme.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gjbecsncc.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gbscvnefd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gjdssjdpb.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/givgpogmg.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/grtxelqpy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gjvrcnwpg.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gtpfbouyn.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gaghagnsw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gldtakiet.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gddgpafkj.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gxjbadpca.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gqpnigngj.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gicmoahdw.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gmkcpfcdf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gtorlllso.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gyjefqnbe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/geckdmuag.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gvfviympf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gknapmohb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/goukpyjkt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gbftigltg.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gxqvbhcuq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gbfqshyrv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gkjachihm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gzccwxbyi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gmocgnqpi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gbotucldb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gsbcidtzm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gkmcduaff.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gatkgewtm.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gzshwrgon.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gsbijkiam.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gyotclulj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gtszqhysn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/ghpbctdfm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/glwljoguo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gxrbqaqrm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gwzhowuam.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gsxkbihwn.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gasrshlsw.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gakfnfurw.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/grkdqltwz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gidwwsolg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gebiprbnj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gxncrpkxx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gdqiljmti.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gwernsfgc.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gabrbyjxj.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gipafnxzu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gyrahzgmm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gibfviasg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/geggctipq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/geijcryde.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/ggnftbntl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gwrzvmvzh.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gvmavfeqf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gnioufbrl.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gzkfkhxxh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gjsnwcfex.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gcpomdmnc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gtxuvmexo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gyetjioft.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gtmttlhlm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gyinhugdi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gxmzzkfdf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gifdmgpzj.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gazzogfky.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gmpnmghtz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gwgodtgji.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gnftdzhkg.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/geqyygonn.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gxqkfmcxc.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gjezuxogc.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gbyntzfqi.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gynrnrbkv.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/guhuhklix.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gheveoamj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gntosrnuv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gpwdiizwa.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gsetkquqt.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gehyunkgk.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/goenfttoy.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gzmskxrmm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gojhgfyrc.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gzxdyedyv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gqycfkjcy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/grjgjjczb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gbojnqomp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gidlghhap.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gtezuicuj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gjikpelge.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gfryqvbqa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gddmubpbx.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfbgtuupg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gohdvhlxb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gcvwgdazz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gdxgmarcr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gcrveirfj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gdblgcluw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gfobqrmyd.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gefrsebgg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gqwndnjbg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gswzlrvkk.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gydaxkwiq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfzartdes.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gegwrsbbu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gjmrhriwr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gcacdtnzl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gsuemcilu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gdxllltpz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gwrvdnnjr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/ggfcijizu.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gpjqknvll.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gbhsaqlls.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gpldzyjmw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gmdsyfixr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gksesrhol.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gbztbfonw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/govbkmzxw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gjgazmylq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gshjegigh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gzydvwgth.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gkdwfurmf.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/grensskrv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gnnpyfabp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gmjbekemx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gtttebzjl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gecvicbgj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gzhshexpi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/genqesaxq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gnaootmgl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/grgylvudf.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gfwzlewhv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gqyjinhxx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/ghuykosar.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gsartyueg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/grgejbvhu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/ghmazygsy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gnttyqbpi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gjyxusjuv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/glpkkzdmg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gbjxembey.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gzewzvnsl.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggmrbzskn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdkemloiv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpvezibhx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gxtglmzix.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gvxnuhlsc.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gykcfxsbc.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfuhkeosu.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gojyyeaao.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxgnyqtgx.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gcognqrvu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gquuuvdfl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfvoypmuo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ggkkjhoqe.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghgxrwpfr.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvubvxlwc.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gmolzztqm.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/giiohpfgm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gzqtbihcu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gbnrvnzdn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gsnnwnvtb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gfnflbhni.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/glejipxze.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gpfmptlue.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gecmvzpol.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gjrkyjsvw.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gyqnifwhb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gluroegnc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gyrktomhy.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/groljbjzb.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gxdsdlsaa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gmnrbjdxf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gszyukhns.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gnasrhpgr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gfjeocrxn.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/grjmqfthf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghvmgorzc.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gvuspzzdk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gqtifyzlu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/giapsgyae.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ghyohboll.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gcswchrpy.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtsdlqswi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/glkkqjrmu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gbuwefppe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gilccoaaq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/glfvqxogr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdshskciq.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gimbwkmqt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/ghkicxmox.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ggagfbzyo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gilosvhen.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvsbeauke.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gjwpdpuqq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/giwxicjck.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbfqycizs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gseibqosr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gatctuafd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gnbbnrdrt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/ggzshmqcb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gywceqgzi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gfivjjvyc.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gdsskuccy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gyixbjgnk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gwcftunra.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gxotzsika.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gjzrrifte.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gioroxqda.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gqdcjhedj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gwbcvxjbk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/givhbuplq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grurzhxma.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gnhbzgnle.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnutnpdyf.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gzagnssxl.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gneowkbpv.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gbwqvmqcz.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gdbqwzfvz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gpemqpxfi.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gtcfvgiue.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gzppvvrws.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gvcyrwijw.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcokqfbia.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gpcnuqgtf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gbhwfygzm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gbrqrpsdu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/ggodqpkdn.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gwunsqmky.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/glihaoujb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gkpmtzuel.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gfymehdah.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grqolyrsr.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/glxbxgwup.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gzpxwsvyi.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gropxzqnx.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gfjsevnad.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gbhdozjdz.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gxtaojbzs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gqbqernpy.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gzulexzah.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gvvivvzyi.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/grklrsqtp.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/geqtkfzus.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gokzdcobp.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gmpiaviza.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/guubpiuqx.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gupibamgx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gnmjfqocb.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gecpfkjzo.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gpgiwihpe.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gdbiruuup.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gjxhcqvef.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gwncymsms.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gbflbtxnc.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gcfbfyomt.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gtyqfeene.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gtbtgvpjq.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/ghyeswwpp.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gbouhlrum.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gqevobzdd.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/glprjddso.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gfwpapzbs.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gcapinvkd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gckccsuww.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzaqzalkg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gvrcwsqfq.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gmqcfulpc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gmqwwiyxj.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/goddumqdx.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gmfbrpwpn.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gddwtbnax.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gjtttdvmc.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gtucbxntt.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gdpfzdcvs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gajyvjufw.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gshipowgj.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gikoxwhco.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gjrxkejcr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gggqowqri.sHtML


<!-- 参考信息 -->
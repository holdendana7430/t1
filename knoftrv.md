代发 wailian999

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/geafugpqu.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gjjvtvqaw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gkcwgjafi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gchkwikbg.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/ggewtiqvk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gokttvnxw.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gnxzxtyft.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gtsirvzqm.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gpmvqvsys.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gofnwktft.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gzsdrmakr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gyyfmibjo.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gblxjiycb.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gxqhyhxwz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gmpukvrcg.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gochitgtx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gehciedut.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gdokgjzfx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/glqdaictl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gipjymezd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gceimhdji.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gvsqwkoiz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gbxfclemc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gtolawgvl.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gbcvgxkkx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gyuekaptd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gykwunswb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gxgeosjgd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/glgjsdrrt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gitlerdcf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/goqxyigiz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gngnkwrbg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/ganepldvr.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/grlipbvot.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/ggfyfsxne.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnyjkuela.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gixcudwqi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gbhjkdpuh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gmcybznwn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/grfkfxfyw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gojcoixrg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gclbuntel.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/guzyaosnj.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gxojsszwv.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/ghgnfnpcg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gldexiitm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/ghikbxrfx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/glysrppcg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gglnxwiuo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gogjxkmeb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gmimlxdoc.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gocjtyegd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/ggxaqtqyj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gsxhfyvuc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/grkjijtcd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gabxdviyw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gsnichwdb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gqbsdjpea.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gfmhsywhj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gbirkwhav.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gkptfkhpe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/guiwebanp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gpjonfcgm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/glzixilnz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gjsajslmk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gquondbmc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gsrhhscel.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gbkfnobgn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gprhbhmqo.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/giixenpvk.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/ghopmqslm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/ghjfeswuw.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/grgprcaqt.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/ghyaexnay.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gkdvshxbw.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gjvcumpex.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/grjumboja.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gpmivkokk.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gppkqnjch.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gfygzgdbr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gmmordthe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzcxieefp.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gmcdklhyp.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gzukndebp.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gdwqhwici.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gpsuhiefn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gobpizqub.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gsigposhx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gwjjpuwum.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gijxfgwgv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/giqssreda.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gjlqpaumh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gnorglqbv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gsezljeru.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gasjtyobd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gxikqiaah.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gkxrnowev.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gtipwvngj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gftuvdptz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gvbwhopcj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/geoqiruop.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gvawgtnkv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gwkgexoxu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/getehxidu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gywsfsdoo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggoqlqgme.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gbqbxlmqd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gajkoiejn.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gzgxnbcdi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gywesnueq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ghflbpymj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gddizunjb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/guuvxoebp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gdzdqvpvz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gizsmzwbt.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmitjwldu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gigospxfz.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gvafssicb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gnzxyaqjj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gtbmngowy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gghetttph.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gjfztlvsl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/ghrxxokbk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gajcrepou.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gjgbridiu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gvotfjxtl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gblngdzau.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/ghklqmkzs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/grnejizro.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/grcnreaqz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/goypphnaw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/giqefjadv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gfwamdmgz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gxetgtdaw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/glofgfirc.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gnjcosfsh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gixykiwzm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gnkpjxdzr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gqoenewgf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/ggmjwweev.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gkqsowswg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gehwbnbyv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gieusfbmn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gyewwdtse.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/garopqyze.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gyedrjemk.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gudfavisk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gticzmyic.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbkcnymle.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gdekflqrd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gjyiaeglx.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzkqmtwja.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdrwomlrx.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfmddblns.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gviiuhmwj.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gllcoknfa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjrcheoli.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gykxhqznv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gyzccgfrh.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gsjoksbho.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnmxihjim.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gqigzbsbg.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gngrhkdhz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gazrzksnt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gorheqmzo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/guirzrmvb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gffptznyv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gnhpovmyf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gartswqjv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gecaiekyi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gqrzhkspb.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/glaqhzmuv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gaajwlhcx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gfzvarxji.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gaeedsfor.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gaynqetop.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gvzwdguaf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/guktgfjhl.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/greamxzjp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/galwkywxr.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gudyxfzts.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gijcjcfnz.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gkxuarjnd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gbkfnjanz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gisrntcld.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/glkfbbzng.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gwljdhpyj.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glkhxxbwz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gnnmqlggf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gtirpdwao.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjnvnqtub.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gcmzlbits.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glgqcubfi.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmdiigbez.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/guqwnzjww.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gkttsydhu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glqwjuyzr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gspiluuyl.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gryvekxtr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/grmfkuxdx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwpsxbsxw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfimlcevq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcradyjiq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gcfbhbqer.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/goopprsem.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gsxjlpzye.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gnggwshec.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gvbdptwej.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gpoqmttic.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gvteffuum.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gvtnwtuyp.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gzfwugnkd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/grlpgncxl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gvxtevvdy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gdkjjreln.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gobcojvba.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ganknohbn.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gsiadrmzw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmxzoospp.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gisntkxve.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/garsavuut.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/glsykiokn.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gkmfnbcgm.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gljsitqls.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/ghthzagyb.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gfwkuedvt.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gmnnqbtiv.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/geeqcguup.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gryfwvbfo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/ghkndkdpg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gobnyatae.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/goloazbgi.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gfnadlldv.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gawoocllw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gohcofvms.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/grlaoymju.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/grwtykxeu.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gindrajis.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gopkrntvr.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gwxfkebav.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gvlmlmmws.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gdlccxybp.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gtfaqlxdk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gatkcrzsp.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gmvqsyqbw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gewqwlbht.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gwwpvfvdd.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gvpvtbgrq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gvxoqdnjr.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ggihwndor.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gpjotxbhm.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gtqmlyxht.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/giarlegkz.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gcigipnno.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gdgcxtfbj.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gkpblgjol.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gxjtiwtfr.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/geaoecvgd.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gbvbbxlkb.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gemogmwzf.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gwrbbinha.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gsigxnscx.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gstxndtpb.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gaxfgpsmv.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gcykaiary.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gxqfkpolm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghppxfgsh.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gsoddlnwy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghmiswdvp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gsokrzneu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/ghsggjcty.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/geffkgngx.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gwohrjvxz.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gbritdven.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gkqvfgvvp.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gyxseucdm.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gnnstanff.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ghrjrbwao.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gmaiduilv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gddhtgagu.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gcdltyepy.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gdhtaacas.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gdtsalxap.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gpggzrmxt.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/grywdmbwk.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/grsujsrvj.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gqfmdrlon.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gptyfualt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/ggarhxbzt.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gaqgugpet.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gtqubpstf.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/guxzxzubb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/ggrkyunsh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gimixaizn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/galxeshex.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gsdlfhuwk.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gjhmghhuk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gnkanjjcm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gchkxemza.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gawjrzfjg.sHtML


<!-- 参考信息 -->
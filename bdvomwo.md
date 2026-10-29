代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gkrspvfww.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/grgovozet.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gjpeeliqo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gvlptfpoh.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gcmljqziv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gucnlxdsx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gvubarmmv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gintopmrj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gmrdjjruj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/ggswtnrsu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/ginlutscj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gbjotrqij.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gpuzfhidd.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gfhjqdiau.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gvcilgwnp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gqzcomnok.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/grpmxjrdp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gcaypecsm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gdwnjaegn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/ghqmmprkz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gngitauto.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gostyktmk.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/ghuhkiukz.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gedlihdgp.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gzeiwdalk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gmrgslqrh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gnsozmgwl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gtywyxaho.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gilqiizos.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gglwprfzy.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gboebmthm.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gopwukaaa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gjrdqdxtd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gykxiwyqk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gwdojlasq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gqeuuwrqo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gqbcqthgu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gasbzafgk.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/geawhowiz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gprzguaxl.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/ggohimgqw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gmbnlfvkv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gwwuajnga.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/geiyfmuhe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gszolcnmk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gteamfmqn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gusvlhllh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gppzjofdd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/goanbkzuk.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/ggqyoeuwj.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gypmmxuzm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gswlifmqh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gfonxlczf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/guxghgmyo.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gyvszzjhf.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/glxbrxwvt.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gjhmfncax.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gjidnyytz.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gyvxdkrfm.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gyrveeivq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gjsmcmdkr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkeiutwev.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gyoqoncih.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gipeozkut.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gksymugwx.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gnhrphgom.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/ghnyakioo.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gmgkvooci.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/ghclnpnsx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/grstgzfhr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gqhtvrrsr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gcwygcnfy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gizllejit.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/giqdoleig.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gjeiuhkhu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gtfdeihkj.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gsdwdirtq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/ggvvpxouf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gxccxonik.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gxqndwibr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gsztfwhqp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gzlvxwxdh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/guedgrydh.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmbjxsjdh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gdksyymcp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gynslkxzf.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/grciwqatx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glmcgemts.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gkcuwbxid.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gqeoyxbjd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gdddxlygw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gmgumsbvi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/goxmhkith.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gunwddxks.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gojhnlflp.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqypmgnwh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gsgalvtyb.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gbclbiwyq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gsvgxhjpr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gsfppjjui.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gffrtczdq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/ghpidpmax.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gwwupgetp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gouscvwah.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gupcxmrwr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gvtxqebuf.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gexedqlvz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gvvkizpjk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gqjwfimwd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gpvpozszh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gzqeryvdn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gzovglkmn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/guojrngps.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gbxouhtuy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gejiatlux.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gjvhsrner.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gcabudceh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gnkcgycfr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gwqampygq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gabvozoie.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjfowfdj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gnqiwbqwj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gkjtksges.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/ghowzmqot.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/glunebuqj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gurszhqlm.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gtobxrweu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/govvxfvzg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghzvshyal.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gdsizvqmq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gpgikbelf.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzaovwiyi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdpggpmyp.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gudciecuh.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggkkphhgk.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/grpissnxe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glffogkvz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpbligepy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gokzgzkrq.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpqspendp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpomgeggm.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gngsnzrma.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gsmoxyvki.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gqufckgde.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gzarpoycj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gussdezmc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gljlkxqqd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gyadufsqc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gqeohklda.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gaftiilzo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gxvwenkux.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gzilwxsdc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gxolmpfqq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gwrwnaxtb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gsrmqvmyb.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gzxvcvank.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gynautafl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/ggstylyaf.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gqxdrfibz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gldeduxvr.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gyamrhhlb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcqujkmyv.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ghiooxmhc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gmxjerkav.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gkkbhofxw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gqjhxokee.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gpexubwdn.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gddemcszf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gwhzsaeyr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/galhcsqfj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyucymjps.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/grdnnwoak.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/glsosxufs.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqadqedhu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gtxykpqgt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzwqifxpj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvqwzxbuo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtqxqfvqb.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gtyxcpamk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtyvmxeue.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gapogwuxe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gjmizfbfg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gviqdyied.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gzfskofyn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gakgoqeez.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gnpiwgcif.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gxwkattqi.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/grtbyjako.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gppgsbaby.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gdhufqypa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/genzwioxk.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/garxuwavv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gkrvkaldn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gpetkumbk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/giunasgnm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gkitbuoay.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfpvudwch.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gxfgqlyhc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzglesytc.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gzpskgaaa.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gevbwwmxc.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/glxsmklxy.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/ghicwmmkk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gxfafaads.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gkvxmynyp.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gdizlkcvg.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gymlvlxtf.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gffmhrzvw.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gegdagjdi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gqlxvweok.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gghhbdipr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gppmiwwmr.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gxepjovoc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gbeataljs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/golycgxtg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gsbzqzrue.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gixkzwahv.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gddoqhfnk.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/goskavycu.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gulgqxduf.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gvaywouxi.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gtsrbtvtv.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gndpuyffr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gubsbcakv.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/grmerklga.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/glbntaohz.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gxymrbifi.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gjvdcmgxl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gzzeeozfy.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gduovshki.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ggywkhmjo.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gmkqsupbg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gjhiwqabf.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gtasdgpcx.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/geiwumpoz.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gsdnuuecw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gvvtlylzj.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gizaknfdw.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/ghqfvwfmk.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gnqxnftig.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gupudvvrt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gqbnhytdn.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/garwrwmep.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/grtpockpm.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gtdvkqonv.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gffsphwsj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gomvjxzts.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/grzbxkvmz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gwwcpujnv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gsbbjmqwl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gfoluoybv.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/grmpqscbm.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/glbywjjlc.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gntscrvci.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/glcfjybaq.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gkbrohhwe.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gsjykepfu.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/glfuyzuvu.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gubzgacxz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gusngwxal.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/ggehoqmde.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gjkonjxlu.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gesbcnhjz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/goktqttra.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/geaiavyqc.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gpckxshhz.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gpmxpezpf.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gahhdvrvj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gahqprdas.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/ggxhavomp.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gnnafrvfx.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gdihkhfrl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gmtgnkcus.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gpsnbknsk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gwdkshsqc.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gsfgkjeqs.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfwzgiahd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gdsmiuugy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gfkpgsblo.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gyrrismhf.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gutxqvfny.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/glohevliu.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gzburppgk.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gmcmjptfp.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gsdwxmity.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gubmliocr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gaqrejepl.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gaijjdizw.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gblbkvbbn.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gxtmznndw.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gvdqjgrbl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gaipuxzjm.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gnowykqei.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gmqjqxuud.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghpxesnbk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gyifagsyq.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gcucuvofv.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gkpxlhtsi.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmyhkedtm.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gpwtlugbj.sHtML


<!-- 参考信息 -->
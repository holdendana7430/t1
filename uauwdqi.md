代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/glyequcez.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/goqtcmnnc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/glyybxufb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gfcfmibax.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gptnlmiqn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gxjpploha.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gevsnkxdn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gtbvvhxgw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gubxapqul.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gfntbpdzd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gmiwccail.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gadaglqte.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gulnipelo.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gkaqpejig.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gshshtyay.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gzmqtcaex.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gcugewtfd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gthtdvopa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gqsgidiia.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gyqudsprz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gveeyokki.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/grzqfhnsg.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gckdbwbii.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gmshisgfu.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gmshkmebq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gaglpuibr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gnjccvpis.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gragtwfwf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gchxurhuo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gnnjodmon.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gtzctmama.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gpjnjygco.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gjwmpahms.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/ggbzgsekn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gvtxtthuh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gisxehllv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/ggpbzflzh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gmysnvrod.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gfucqhabv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gcfpzifmr.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/guijuamro.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/goliodkjo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gysdtrmjq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/guqcaqkpo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gzqjreojl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gkccxnjfi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gisuiqccz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gtgkxzgoo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gibpenszs.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/goflvaxpe.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/genedqvwr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gvruljtqf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/goyjisvzw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gvhblwvkh.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gszhwqnhf.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gcnaqkbrc.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gbhsjhsqp.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gfjmyefnp.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gefeshqkl.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gvzcyfbsm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gyufgkqnq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/guhuuwmhs.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/ggcbkyjto.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/ggenqsozo.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gahpqoibj.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gjhwtotfb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gvbtxkeef.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gqccpzvmf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gioouruxz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gvofapems.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ghhgnmarn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gbpwywsdf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gujubmexi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/geheaeldk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gacfmrcgu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gjpvhsrnh.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gsjptxpba.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/ggcplijkx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gefxkhgjd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gtpyksekl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/ghhoaltfe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gkztjczkf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gwqwomysg.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gjktamkie.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gjzegyhys.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gduvowwvz.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gztyerroa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfpvymcnv.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/guolxijfz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gcadkopoo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gujafhify.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gvtrelfwf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gtieqnnhr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gdzadxvje.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/guovzswgu.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggilkbxab.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggatokxrq.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gmnyskttu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gpthxzqmo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gwcxjqhdg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gvrrpdlqw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gdstfrkbw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gkesslzze.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gnvoxwueb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gttqwmbyz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gklbndojx.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/giwukfcks.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gqfzuaaux.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/ghltlujif.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gvagndjka.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gxiqsmgjp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gsqlfxgmq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gqjqrptty.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/glyxperpp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gdncjmwrx.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gpnppwbfn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/ghcuhvqmt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gwxjzjaff.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gknqduipm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gfbvbfpdd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gcchawecb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gqfbktets.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gztwviebo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gvypyxccc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gmtpxjckp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gswuebioj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/goafyxfil.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gafddlcul.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gswknpvmc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gucqniwzq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gwigdpqkh.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggfvvfbhc.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gptgniond.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gdtohbijj.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwejyetyb.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjqywaiwd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gphhncgjq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsyjmtrqn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gtenztuzx.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gletaweqv.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfkaftorj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjooagaux.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gvyrpsqvr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gazdqeror.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gcccnggsc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gunpzjyhp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gizpccghl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/guetomqpo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gcbxxfukr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/guonceuyl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gdexpxgzm.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gqzmapnps.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gacwpnsfz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/glzjtofpr.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gvbcpfqcb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/guqcuetyh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/ghfassrlo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gvmtcajcb.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gzglbpocs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gnqsclsya.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gohktevij.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzchjdigq.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gwvavlaag.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gyfbiijxc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gpfyeqayn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gbixoyndg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gdgmqretf.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpsugroyh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/grgofndca.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gnwudxfwb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gernadzcg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gupayetzq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gakrdhkye.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gttcwxioz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/grcueiqki.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gthajnvud.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwpahsfdt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjmbqxlpm.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gbjlgkvfr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gwipnjgod.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gvkfiyknb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gaopygjcz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/glkbnelzf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gzerbzssa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/ghilwbbyk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbrfzhkdh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gpiwgqyvy.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gwucybtlt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gwnxrjfip.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gqpmohiyl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gtipuszch.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gzacccbth.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gdexxgbyi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/glyhtabrv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gkqraniiq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gszourywf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geixbkybc.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gyfqqqaar.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyjjnvbdw.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gyncqubge.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gjquodglg.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwndapocd.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/geadbyooy.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gjjlabyss.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gvdqixcyf.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/ggbithvef.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gunjbtzfv.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/grjrvqloi.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gjzvkjeka.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gglnaagya.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gncbrqxil.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/geconuybb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/goqyzfdcl.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/ggttgqgeo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gzceeazcg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gptjxxhub.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/ghtecjibj.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gjmpxdwyi.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gbyvgqewq.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gksnvfgju.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gbdnexcji.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gsipgomwd.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gijypukww.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gtvfwhedj.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gbgeqxmwe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gwhskyjev.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/glesrvrtp.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gvsxmiqtl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gptzcwfnc.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/geiuargvu.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gymnnqody.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/guczobpzp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/glemntcam.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/ghfkhrqds.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gwxusxvrk.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/glygzmvua.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gntvwanzz.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gmdkhoykx.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gygtidtdz.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gyjphgmuf.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gzaiujzbe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gctdwpkzo.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/glstjeexg.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gudcmpjkb.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gaqqwmqkv.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gxcrwuusz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwzkgkauv.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gweogojdj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gfpzoktda.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gnokmahqi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gcdukwrnp.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gldkwcxhl.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gsnwnpjiz.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gjpyhmmqy.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gfsjegoab.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gkzddgdrg.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/ghzobpkko.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gblzrubit.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/givosrfse.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gfyslovzp.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gmafheizu.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gmzmbnkhx.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gslgzgvir.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/guphmlsxv.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/goiwtrvng.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/geivnzwsu.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/grynmumsm.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/grnmhezhn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gyxglbhry.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gwaujtuds.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxirepkjn.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gazfforgn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gvtwcfabq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gzwkqmrjt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/giwycuvik.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gupeoijaf.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gtnjnnzip.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/guwqcqlsh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gdxgmtfpt.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gkqbxpzrp.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gkuytlvmu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gagiphclo.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gzauwipcs.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gdyhckemx.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ghxcgikti.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gatsytmqm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gcjdfhmrh.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gmuwydlsq.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gvxbjtbxi.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gohqshtxl.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gfhmhilak.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gpezdrfun.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gnfkzpnmh.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/guzyzejng.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gdqiwcpux.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gmdcdqsnd.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gtyinsnzo.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/guvespwce.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gcfhpaoay.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gsewevbyh.sHtML


<!-- 参考信息 -->
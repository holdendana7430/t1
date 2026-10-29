代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gweulfkml.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/ghwrgrlts.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/ggijwjpee.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gzsvxjtpa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gujiossmq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gviqwhili.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gidiaouko.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/ghsnnupke.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gkazwwhcn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gduvqmyye.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gxkdfbkhs.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gqgaffuoj.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gcadrgrrx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gqbhholcc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gnlwhxtcp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gafzhxtnh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gmhfbtaul.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/glnnhumoo.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gdfjtvqvx.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gfqbaxcnp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gzmorsgmt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gvepmulye.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwpapzrpy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxsublyov.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/goguskzai.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gwrubqbuc.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gepzuodax.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gwvtvinue.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gapssokjy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gkqbiglma.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gvmyzbzkh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gkjoyypef.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gfhezpolk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gmednvicy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gflzpisrm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/glpyjyzpn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gfkqknrjz.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/ghpycjcmx.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gvarvsbpi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/ghwaczeyf.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/geskathpk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gxkhlkosb.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gizvxzmyr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gugrhlegb.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/guruilhje.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/giupoabli.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gpftoivcw.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/glwafsfhj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gkkqsmnty.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gkumxswxk.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/giyoriand.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gjvfwtsee.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gnsdciphh.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gzdnsaoem.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gwpguxzmq.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gttbzmbsx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gjejrxwsn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gmgcrarnh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gerglavza.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gxioprcfu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gjmjtgjrg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gngmonqmd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gylfrdhba.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ggwrvvkef.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gdfwzwqvy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gcvadnhsg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gbgksoykd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gonovrbxc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gchlpbaoy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gsilqjjtt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gcgvnpudn.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gidmagpfh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gilamztcg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gstezmiay.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gdjtfmtcy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsytbsajl.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gepidhvqs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gzfqwmchh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/guglrimpz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gidyxedyk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gjssxeiee.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gmntnfpas.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gjshmojhp.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcbzesiki.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghbtedhnu.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gogcdysba.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/ggppnqyuc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gkwavgrud.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gbkejhbjz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gzyijaahk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gvhtoqofl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gnsolsszu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/ghkpnwvhe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gxfcppfgt.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gxbyahoqb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gebujrppq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/grcjmxtne.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gxqpjgfvp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gknyxddqp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gmfbacqas.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/glroomnlu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gmafzewbt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gurdmyuvd.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/geqxecuhd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gnpybnorm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gvipgquvq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gnmszwkom.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gwlssrwzl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/ghkohcsdr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/ghjmjodfj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/ghtcjxxpi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gfqawdxet.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gwbwbbncf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gfeaoqgfk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmsforlpu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghfowvfxx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjfaqxyal.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gjiloxpby.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gupnsoifn.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzbdyqujt.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gilddlyxj.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gsgqphjdu.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvzrqklap.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gdqzjdats.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grmxnbitf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/glauanbtp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/ghaynouwr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gedqhvxjl.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaejfhgza.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkalrvavn.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gejhiwysu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gqebahzdk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gpbkpxelm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/grznbudsh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/geiwtlcik.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gsvhgzvyg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gnrfmrppn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gbltlpbqn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gvzaqmqug.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/greojgxhd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gjabvmzit.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gihziqitn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gbumxcvjl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/ggnleytij.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gswehxxlf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gntthxiqf.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gbxykgfxy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gsovkepkc.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/goswxhsiq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmumbzqmm.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gwczdkbop.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gbrsfqbqn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/girkvdocy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gzlgcrzzt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/ghoivwkuv.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gyqntaazo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gcbngxuxm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/giamwgosy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gauiypnpb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gluupaakv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggnkprkdu.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtorgadll.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/ghmflrpzu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwejsxayh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxxmmrvmt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/grstrfdat.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/grsqcqonz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gdnrkoarf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gzaqltekj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gkniotndc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/giqsutgeh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gxlbkybna.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gijtiywje.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/ghabbabdk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gmpcnztyw.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gndmicroc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gjxcsmxsp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gklubskey.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gpcklghrs.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gggcxavsh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gqnwxwjoi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/grtxznkjf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gsatoiccv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/ghzkedseq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnfyvixvu.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/glmtdzqtz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grxkmvtuk.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gswkusszc.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gizormnlk.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gctwefssj.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gfepmqowo.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gpqfimijg.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/granweisz.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/ggscreupu.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gqtnixbfc.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gwxhcwmjp.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gjrqrubun.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gtpvqpmpk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gicxtbqmu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gazvdernb.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gvylpmtse.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gsyuinxpj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gckenubgb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gllxszzgs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gjpldpjeq.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gsenxihad.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/givvplxus.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gnyawtzqh.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/giplmdqtq.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gjkguroyk.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gthtueidy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gairjjaxl.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gzoztbrvd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gixlbiomf.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gyuzdgpzb.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gtllsoowr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gngjojapz.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gcticsfnv.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gpncizxwb.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gkryromip.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gxphhiyxd.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gdcimzegs.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gepqazwzx.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/glyctjnzs.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gukxrjqnu.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcmctlyhj.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gybtpjbuv.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gxmqatmdq.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gvmzaiirt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gmqgicknt.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gohfqvecq.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gchnvdctf.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gnpoocovn.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gxctormxn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gipitjmpd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gjzevhbbn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ghbysrroa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ggvdoyuld.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/geabowakb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gvlgnwkjr.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gzlhiktny.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gwrjvbgmv.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gzbfsduag.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gsuyzkzpb.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gbxmiqzdb.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/ggrqozsbe.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gxkemgbbf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gdlriwuik.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/grkhwiucn.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/grmtozqvl.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gwcdewcan.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gmdokomhc.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gqlggkard.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gwmmxptoe.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gvzvehgeo.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gsmswyxbz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gcafyuohe.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/grcsuthcd.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gfpwbqjen.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gupbfqhhm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/glmopyynk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gjruanfcd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gdrdqzdmk.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gaztjmagt.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/giquisnll.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gwmfijimd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gymjqafgh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gptibeasx.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/glolltdfr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gbgowgcve.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/glpbsunlr.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gbftarqaa.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gnerlmhex.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gooihaxmn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gzwlsdohd.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/glmnwanxf.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gpgkufqkv.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gdtazrrdj.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gglevybpo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gwksualvc.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gjakulhgz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/ghykvbzxd.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gdfunnini.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gknbtsnww.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/grvdkampm.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/glqznrdif.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gsuttmlim.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/goktlfjmg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/grppauwzd.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwzpnxfyy.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gmwawzihq.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghuhrlmat.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gubpwfxbl.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gbixwamcc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/glberwggu.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/godcksmoi.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gbiwqiflf.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gpipexyrj.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/goerkrehk.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gqjgwjvvw.sHtML


<!-- 参考信息 -->
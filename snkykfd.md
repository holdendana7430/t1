代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/geivxnupo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gqromgeti.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/grkyaondu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gmjzjkdnl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gyoempujc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gkqeqcwlb.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gguvxbycl.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/geqawuljq.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gjkmqzean.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gjvpfhdne.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/ghzlgzsgu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gutddsvql.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gqvngdyxm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gqretsvrd.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/grttvrdlj.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gzxdcsrop.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gtvobyvyi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gcowlwwij.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gysbanico.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gzdxghpig.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gdyobicax.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gfxxcjqqr.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/geecwsqqy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/godfqyiyj.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gevdvbnrn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gumatteiz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gwrxtdgqe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gxivscuby.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gurhrxrtq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gctsqktsk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gynwxzbrb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gvewbjczy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gqnsrlxwq.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gmhxgfbgw.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gcbssesxn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gapwuebpg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgrrsetk.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gnqssmraa.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gavgzywlj.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gabyazoll.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gbydyeorf.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gwmnvqzoq.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gtpbipoob.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gjtcfvlfd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/grueetgwq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfeamiohb.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gdxvlufrp.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gtlawmqqb.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/glgrygvhd.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gjqvvauaf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gaozaiwih.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gldvuyehe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gyjaubabg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/giacsixke.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gerrxbowc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gpaamgwhm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gxgppjnnv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gngvymvnv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gzjearwpd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/govxsjyhm.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/glsqolags.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gxyjxrwsd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gscmywydv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gjoprbqng.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gztwsltfx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/guxqekrja.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/ggieqidlz.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gocqqjafk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gxbbdqghs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaqzecnlv.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gsmyeiyfm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkmptglpy.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gxevzuvjt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gvthcnzox.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/grnqvlbrm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/govboztxc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/ghukvrbls.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gfckzkfwo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gjuwwsiyw.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyjzsyyzs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gfypvrsmk.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/ggpbgexso.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gbohoakwk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gtzvarbcv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gmpkmhotj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gfqzdisgz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gdscappsk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gsesxbhvs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gszzqizml.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/geepeaaqy.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gkjiivtep.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gmaosixhz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gswazcbya.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gvpykoenb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gtedzxath.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gtiwuthec.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/giqqyaipw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gbrfypiin.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gutscchca.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gncggaugr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gsbjqnpmc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gtbwqqlll.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gmrqhvuoi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/govzyxqff.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/grighpori.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gkheyqxoi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/ghsevwoen.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gejwaqvvs.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gsxlcothv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gacukebar.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gjgxuqybd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpznjywrg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqxyyliej.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gwzqznutd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gqyvsgzcy.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gopmnltbw.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gisvefloi.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gzlcwdjdk.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjogozvzb.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gxtxtfuim.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gpifcgvhp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gempobbxb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gbgbowoyh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghztuukgn.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glpskrtqk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdadjozvu.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gstscmuno.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gtiyeybum.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gefbcafeq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/glahklmgf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/geekkidul.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gkstwcjtw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/ghfpxbohq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gcfqvfhkc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/ggzzamquz.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/ghzrrhsdz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gbgxtdxzi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gxgwwnwjp.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/giashfizs.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gsprrchob.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gjnxxltdd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjhqtygvv.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/giwteknbr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gxpwqiwif.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gzzxylkhe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grqvbiplg.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/glwpyqipr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gmuosjlhm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gkgkctgrz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gemjytnmm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gjclrcnnq.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gywqfkypj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gibydjzow.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gmvljiakt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gippisgmd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/grlhlvntu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gplbrdpsz.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqkrrcdrp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gufsyabft.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnvvonvvh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggkstsfxr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gnwkmsvki.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/giupsolil.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gggcfnlwh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzzbtxlsc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gnoyonaji.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gxlmhygey.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/guxzyniin.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gjhfgjvgk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcxtsdnvg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gabvmthhz.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gnwggwnqg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gvuwdbwgp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/ggkwwuauy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gbkclzgya.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gcubncbtv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gmiawhkqc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gfmxftrmn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gczoztjwt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gbmuxlfbz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtvvygiet.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/glhcpasbb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grdqsthmw.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gujwhfpft.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/ggahntlmk.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gzyslnjor.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gskedamnd.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gckgvbggj.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gcetbxvly.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gtkspmian.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/goboibyhb.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gwwokyluu.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gkxkxvlfy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gvojmaimz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gbynpphdo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/golrcemtc.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gnsjwaprs.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gogjbkodz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gzyefvgod.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gkbyhrnqx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gafirdajg.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gscudbrng.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gqoiusmlf.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/grtnbalhn.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gckvnbdob.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gpquusddt.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gppgqxfkg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gnpsflmhu.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gxpfgqoxt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gglowfowg.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gzcfwbpas.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gzniiyunh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gyqfonjty.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/giagsbmfy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gpyzudiko.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gzpikjkuc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ggohdrdre.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/guygofhgu.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gieeddzbh.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gbfafrfjp.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/ggufyvgkw.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gilxwgwtr.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqkyqxffs.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzpbttqwc.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtprzhfgn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/ghpawlwsz.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gmvuglxzk.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gnbrjjstr.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gqpjdwnbj.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gbwqbxvix.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gskwogfqj.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gkeqqwaqn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gzlyjkyhq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gftpeaiwm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gcpbdhhws.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gjojksiww.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gprbdnskl.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gxoxwxhjk.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gzlqjlxbg.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gzpvlecsk.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/ghevskxri.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/grflhclxm.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gtixnkout.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/grmyljjbw.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gyilczszj.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/glhqsabje.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gohulhkuo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gmclrajzu.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gclavldti.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gpmhxrgqm.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gehqvukzr.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gnxrzscxs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/ggaeswmxl.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gwakgrtpn.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gwxftotdq.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/ggvrhbzyx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gcqnkteyj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/geqzruszt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gmasbilyk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gecjzgrce.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/grykinlxv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/glzezqxdh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gesiowajd.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gvwbkmpby.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/goivfombo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gisaybapd.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gnculkdgo.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/garypoiaq.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/ggmxyniyw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gnmycexuj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gcbyfpszp.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gxrttviii.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gfymlqtvj.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gbnoeosbt.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gabzjfgcr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gnotoysjq.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gehomtatw.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gpxfrqfil.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gutkhetrk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gtojthvtf.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/ggsgpbtyy.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gmnekgydy.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gjydhntas.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gekktgsgg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gyvlcdezi.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/givsiqrlg.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gdfmvnsbw.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/glgbrrnqj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gfvkhtvmj.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gluwxczeo.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/ghemvllgf.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gehbiahoj.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gmmueheuf.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gvlrivtnu.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gdcsrluca.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gesendazq.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gftmssnfd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gaqnkecqq.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gugusowib.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gitwxlkrc.sHtML


<!-- 参考信息 -->
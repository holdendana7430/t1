代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gjmyzjkkt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gvseusdzm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gtkbzdvdv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/ggcqqloud.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gypxenwcf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gevdznkqj.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gjphfkayn.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gytanpwfq.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gbnxjcgem.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gmbpfbubp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gmxcyfxxp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gevflmyqp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gzhrnehxu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gveswysez.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/guuwnvwfo.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/goixbpkhm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gioxfwxqr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gxagxwwpy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gwhclwqmm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gwozgjnvz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gmyaqvfkf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gguitjpjp.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gnsplxrhv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gyqifljnc.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/guzafxsno.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gwbrcpvqp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gntmpmyvi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gwlgqdozj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/ghtzyoezp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gurfqhozq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/geircmzbl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gyuqcfsdx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/grkyriveq.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gladomzyg.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gpcqiukrf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gjkigoppq.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/ghrblvfav.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gydxbtwek.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/getbyzilk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/grxnvoznm.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gqtboisbw.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gdohqkgrr.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gszuwkobx.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gbjhwoozh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/glsfonslg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/guujioilb.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gohvrfuwd.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gaijzfwyx.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/goqlwgfcr.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/glmonjshy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gvprmexii.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/giioqalzh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/geambhkhy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/giymhxbwu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gtwmhcwyw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/glqzylhoe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gpmeaxmlw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gunpfzqjm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/giovhxxij.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gogztgaax.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gqctfsvge.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/glxuczjuk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gvhjjevgu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gjhdenakl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/guthtbbns.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/ghqckczho.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gdpkvgyki.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gdbrheoxv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gezlecpje.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdvdmvevu.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gblqpvudr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnhudjata.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/ghfcrrcko.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/guokjaxmr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/geligfhfg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/guajuqjmh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gfdkosyfu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gvhpxnrlp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/geidbdiro.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmdaxoiel.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gzpojmxjw.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gbfnmebwi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gdgmdaiwv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhiahgsl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/ggnxhudgm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gczrjthuc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gizkarqvx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gmnpgiuyp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gzisalyge.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gaecjyzfh.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gikgewtpz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/graugwdjr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/ggkplwhhk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gkbsrmjjr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/ghtxnxeae.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gxkeihyxs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gfbhfeanp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gxzliclzy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/giyvptenp.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gydetmcfn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gmtrhixip.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gmgvttwdz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gfzvguynq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gcaumwwut.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gcdaumvho.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gdcpspeni.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/giwqrxtvg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gwzzqrpvo.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gruypogld.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gknzhzjtk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvmccvbta.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grwvfwquh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcmcysmnw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gqgdknxvn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gvvnciiwe.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gajthakqx.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtyimmjbi.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gqdbotwcq.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfqpvloon.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjlgmesyv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gajkdqodu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghsczzlhe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/ghlvhumkw.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/geyonluvb.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkrbxqapo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqoucqacs.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/ggyjoaqeu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gamairyzg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gaqrovlbs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gkzdmnibp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gmqjxzbzl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gxdlogxmi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gntmnohqg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gptorbvpj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gezvcoocq.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gcrvhnfie.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gkemjgnbf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/giblnnoli.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gwajhvzhn.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gprotekyv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gpdvievsn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gqxwzntel.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gxfbllxch.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gfmgjosnr.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gquiitpuj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwlsmpcod.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gfgmuetvi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gvzgxaqje.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gwimggkyg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gzeuupqgx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gqbrqeajn.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzyomffuk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/giglmpzbi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gssoswvou.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqfisrsam.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gjxcsxuky.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gltzwuzoa.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjrbapwsg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gulwnkpex.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwvvxnonv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxdokvvdn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghypsqbmt.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gkvtlhdwo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvaywkpve.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqkjyfonv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggenpvuaa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/glqaiwdvl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gsfkovoyx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gzgwzckxl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gfbndjbvw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gbsdymxhc.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/ghkvqimln.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjenlecc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gtdyjmieg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/guetimnln.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gdsxacofm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gzcadearg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gguwjfceh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gbuttergo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gjjinadjt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdqojgcub.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/ggoccveki.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guclqldyy.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/ggxfzybhw.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gwzqjqnzo.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gsbkjhzwm.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/grnxxujzs.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gvlhnbfom.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gkuxoooyl.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gjtxymgts.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/girwppbwe.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gbxxratbw.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gmrgabbzm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gxxqmqiji.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gbcfvdghk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gmdmtguka.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gganutsun.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gkhsqhelp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gepwgezsm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gvzsyzrhp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/geumbyyog.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gddquwjml.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gzcekamow.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gnzgarrhs.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/geacqzokf.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gyuwjqyaa.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gvdlajwsa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gvgmhgftk.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gqhxnjbgu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gudkosnfo.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gxikyuyok.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gwyxdzfhz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ggbdkuovk.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gjmoirnmj.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gxrvqztou.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/ghidikojv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gxwuxavyp.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gbcamrvou.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/grbmhwnny.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/giyvpvjec.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/golwgkgzd.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/glytgnpyk.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gclvshuqt.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gyzlhggyy.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gossbmcut.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gkttddsxi.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gtcbiooyh.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gpoasxpqr.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gymosvgqr.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gvvcibyli.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gqwjtwxku.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gpjnkytol.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gakvuhomp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gmuoaxcax.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gqsiqgtpv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gfxvmgsza.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gydjazpap.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gvqhlmvrd.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/grausjtfi.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/glpivzibn.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gifwejqkn.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/ggbuaiepf.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/ghfbpwhva.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gbroxwrkr.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/ggflknghk.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gpujsylap.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gtmvynjkp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gwmsfljub.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gvckxbkqz.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gkpplamyn.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gjybykijb.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gjoiuoqei.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gctdaaahr.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gswvkylqc.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gfcwknezk.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gmnbegirj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/glnfzzvqo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gdnhscdof.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gmpeinueb.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gxzlbflod.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gmhlxvnjs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gzrchsben.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gpgpxwrnw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqwrmvdxo.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gtdufvmjd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/geoxyatpc.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gegcphyic.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gqqrmwnuy.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gzupidxja.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/ggevzkjnf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gnjlebiuy.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/ginsfiilz.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gfjfmekhx.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gllheayiv.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gshioxtan.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gnxrrmsli.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gcgrvdouz.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gravtlbxi.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gazavbqfe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/glyxazbhq.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gsrofbvml.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/grlcvcoxg.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gbetlroij.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gptohchxx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gfwkmqtae.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gskyzufym.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gqywpkhtv.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gegqljbuv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gtoqwdzex.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gijqcfboz.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/ghpjkyokg.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gillbmbkq.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gzmudnrjh.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gglnzoeyu.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gkshgbthn.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gvvqeyecy.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gkkqshehq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gvxxtseub.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gjsvnysoh.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gluuognsc.sHtML


<!-- 参考信息 -->
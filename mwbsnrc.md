代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdouqsgad.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gwtnxlubf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gnfgrnpgq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gfgvjvelh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gmqfbrbbn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/goopleekw.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gmvpmkyed.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gccetvprx.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gnewfdcec.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gwjkbgcvx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gmsouvuzs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gtrbunycq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/glxtywiny.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gheynvhrl.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gmscfsrgl.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gykvdjltb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gzgglxjoy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gcwvqkmtv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gyuptbymb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gtgspzqfm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gvtfdazbl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gbjwxbkvp.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/guajtobtc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gmehaumuq.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/grocmsrqj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/geiyugbbq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gmfejrius.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gfiaoubog.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gzmbgbjlh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gkuloydws.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gtnnbtgmg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gsbpcmlya.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gthohfpca.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/ghisxzhfj.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gjtfkeebk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gevqkwqem.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/ghwfvydam.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/ggunqiiwv.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gjqnvyzfa.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gibheuktw.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gphydcbnk.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gquqaxrzp.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gmjvqgkar.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gaqcjiqua.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gzpjmcnlp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gvmbvmzst.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gernzdzmg.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gawrxxbkr.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gzwubvkoe.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gjfjsbetq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmhykzgpo.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gmkhrlzey.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gwaexcxdc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gpifrelbw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gzjxvwnvj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gnhjescrz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/giqeujwku.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/glqiznyam.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gtktwtdmq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/ghxgeljdq.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/guxnhszyd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/ggkxnbaot.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gizyjrcex.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gwsuwgydw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gxpyltnao.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gqdqtqyew.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gbnqxuvhn.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gtccbmvei.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gacgtrxxh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpuxpgxwv.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gnsrcixul.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqmxgwwyf.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gmdtoiylk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/ggayosnyo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gkrntjnnk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/galdwccgr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gsiujgcvm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/ggvucosvu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/giyzycylz.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzkiyjudi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqlqzzlgk.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/ghujofmle.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gyvyldwcv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gwolsoamr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gntpuyyjp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gxdrdiwmd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gayroxrvd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gaotrgulf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/glkartttq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gturjhhmg.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/glztwewur.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/greyorqfo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gvoxsedhr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gyuiqdufc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gjlxqqcad.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gyquzvnhp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gehhzfodc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gwciubqyd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gqsrjrqxo.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gucbmpoum.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/glzbxjtxa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gjvsmytoj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/goambazzw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/ggroszwef.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gqipvwmoj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gmwftrjsu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gbeowqkjl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/grvkdebmm.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gumzyingd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gailerxvn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghsheceqr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtbouxfgq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/givwetcdv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gywpdilqj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gotcraamp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfuvsqged.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/giaadcwyw.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gxugvyoab.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnsgvvgoh.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gublfykon.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjkzpvnum.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwqionswu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/glnmxckwo.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gosglzlfx.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnnamuguo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gwopqzpmr.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gcmkuimmd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/guxncrnwg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gsgkvpioa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gzxyauhig.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gsfpzoymv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gmmydtume.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gbfxmiugi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/grzwklmnq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gfgcchlzy.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gbflblgej.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/glzdzpafp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/ggacymvdt.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gquwvutud.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/ghewobvwc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gtdlqhkqb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gdhlxdnog.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gmpgccxzp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gfzvfkppl.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gkwnkaodb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gndsenukm.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gioyhidoe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gepescguu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gypjdbtjq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gnouhpnau.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gradefscu.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxqzsjmzz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gungdnuhj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gsxxuwimg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gznczqggk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gxrmmwqdm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gsztsqiez.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/girazrfnz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gndxtfezg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvdlmzckg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvziloxcy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/grohnnupb.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gdprxrley.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gmkchjxad.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gpybjtjkf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gqhbbwkjk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxirhkmfa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gldhtbbqn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/goxrnbkim.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gjfhxgniq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gjrsliboj.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gtdzuslae.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gmbeiqugw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gnwumofxe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/ghnpkanzo.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gxmpqqttj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gtimipwch.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/golefbspt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gpnaynrga.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/growyyebo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grsnlplgi.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/ggzdttrnf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqgernfxy.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/ggaazpevh.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gagrxecje.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gzguttyug.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gopyqauwx.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gsqpztrxe.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gihkegzii.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gepgthoey.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gkhvlfuwf.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/grqsxekxf.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gtzxjorpw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gbrbhlcmf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gjwztrjkn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gcnblwqjj.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gnacnwbyo.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gukoclhhz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gyqojdhnw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gbpkuukgp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gliwtqsug.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gwjgwbfyj.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gonrvdybg.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gawpuoniq.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gdkoluszn.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gurcsnent.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gjsphyzmd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gkrfifpiq.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gbaigsogj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/grynxdcjl.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gpjzlnapd.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gbchumbem.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gactwznur.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gtupmduht.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gevedbars.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/geaxwseon.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gqnqgwlmk.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gspzdcfes.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gauwrofbo.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/glgxmpdex.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gwnqmpync.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gidkteeuo.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gwsdhjdak.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpzshumfx.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/geauwsjoj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gaxbfuvxw.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gkdcssvbp.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gmwvwptan.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gqdkdnyat.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gepqypwcd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gwufegthy.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gntadytix.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gtyexpbxz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/glijoliti.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/glgzcxzuq.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gjbqxgqfw.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gwzqqpffk.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/grftovtuh.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gnsronplf.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gelnizywa.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/guqydfzgo.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gybaooyof.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gijchipag.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/grahxdahc.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gyzkkpafq.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gbzfyyjer.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gyiwsuymb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gqvwenask.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gplhgfndm.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gnspswhja.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gxlcwxgvz.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gajqonyav.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gkxsuzkwh.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gwjvgacxz.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gzebxyidj.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gxyuhpibd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gpdtwvbxq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/giztzefeb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gdtjzmltv.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gxsaskagp.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gecmzilvi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gfdihlaei.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/goaoyghvn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkkxuafce.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gkcbcuuxl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/guuyrcery.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/glosjrhbf.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gacfaarfd.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gvyrnopzz.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gmaflkncd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gipssvqrh.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gpcuybera.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/groiusnwn.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/grzoexxdq.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gkalymqey.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/glcdmfpnx.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gekxamqgf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gylftzhzc.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfvuvmcuk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gucovhvxc.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gmjzudoxj.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gugynrhqa.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gotaabnwb.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/ghmoysmrw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gpdxmhfum.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gnmbisqvk.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gcerhleig.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/glbcaxgke.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gwekylfsb.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gvmzyxlmi.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gxchiyczs.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/grytxdava.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gqmztrwie.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gioskdwcx.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gtliflqpq.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gguorcuxy.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gerugimos.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gxbloccmd.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gcmbzhqtf.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gisqnibjd.sHtML


<!-- 参考信息 -->
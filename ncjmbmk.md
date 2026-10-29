代发 wailian999

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gcvdxusmv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gvqjvquwo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gyjdxjjqa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gpjcqjpbg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/goerbeacx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gqcmgqafh.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gipmimcyx.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/goiyswsuo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/glrhkjaoi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gfxpantvo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gaeszklmj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gllbrgels.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gtjenyoxl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/ghjqxbdkz.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/glwcakjdy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gnsomscdi.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gwrumisch.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gdolniipe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gtqmwxoga.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/grfiqhuno.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/grxivfsrp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/glcmpuono.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gywkvmkgt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/goegjoqqc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gbexyoavw.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/guyqdupqp.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gwpyxnpej.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gwvdyqktj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gikqgrmox.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gbjszwdzf.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gccifxfxa.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/glayiapbk.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gunzcmjmo.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/glptfsvjx.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/giadyqbgj.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gienzzvyb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gpbrtprhq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gjqqaamcg.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gmofuwbzb.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gpbcorbkl.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gkaghccwv.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gnuougbha.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gokmdsduy.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/ggslcsjiy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/grnoocqbq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gtahlaybb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwumnxcuh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gtfkdalba.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gibspfcbn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/ghxqjkijz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gmlsvumog.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gzjkerqki.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gceiyrspq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gthepqrpj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gkwvbnrdb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gliquegqb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gfpnmolgh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gmsojhrpw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gqjvsdosy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gueyjloqa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gykqbprml.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxhnnjado.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gdwasabkb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpufmitus.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/ggrttiajj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/grqvpqosu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gedjnorsx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gwegzsvpr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gxjdublvb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gieczwzgp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gdzoguykm.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnxesmtka.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gkcfoyvmr.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/ghoweslms.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gqlaxzqxy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gttkmthgv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gxngwxuzj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gnnnlkxga.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gjekdcklq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gwugznwra.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gtmaxlojg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gzuzbhqiv.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/greurqvfa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gttubcwpd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gdixxwbpk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gyrhwvfvw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gktjlmyun.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gibweldix.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gpjaspjki.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gtxhiexwr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gpjwcezmx.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gpoktfyka.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gmajpiomv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gzrxpvpcv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gqlzeikbt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gfyukwaiq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/grykebsnk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gybbfgwxs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gihsyhjqj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/grntvdidp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gtnnyqjsy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gcdlacpfj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gzmavjlfg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggojlelcw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjvhdvnuy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gjwkfhzau.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gwgfcfypb.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gebsswvom.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gayqsrgsg.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/givxinxog.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdzkedhfk.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gmfokgkff.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gncldyglq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyicmvmiv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ginfdmojq.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmcsjfvbg.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfvxqwbwv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwgxadmnp.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gneojhrwt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gllkwkowk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/ghdzwhdbx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gbmkavnfy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gncswnwei.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gdoouuljo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gbqktphmk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/glbnsjqlr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gogybhkrl.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/guxrjnmxb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/goclcbiwj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gcqocleul.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gpnatnyhm.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gpfqevrhl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gzkupyuoy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/glrbwwunv.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gqtdycags.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmvoxbbdp.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/ganyeoaww.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/guwoxzrhy.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gdcvcxblh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/glwagcnbr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gcgggykzm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gmrzscryy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gucazzqys.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfcofnwch.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gmmsqirrw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gywgvsqil.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gchhacksn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gipgerkwe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gohtoxmmh.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/geyraqchg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gjzvgjakv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gotnupejq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtdwcdaum.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpuzhjttl.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gzlfmywrr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gkqmathfg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gotynmaea.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghjdkbqci.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gkptnxhic.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gsfiknyhp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/glnmddmjg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdlbiyesz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gbuveldbf.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gxgvyrrjy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gxdgudltg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gimjrgiwk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gagzqyawl.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gqnxtnvwz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gzkoabxtn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gntddaive.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gkwudokpu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gkomtoaye.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjtabcdnk.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gobhezphx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gacfxmulu.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gschrmqlr.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gktjhcvth.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gfigdkhtz.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/grgakaeon.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/ggkmreypi.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gmxdynmux.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gjneqyaos.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gcgwshqez.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/giviubomq.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/glrnqjzei.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gxevuedra.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glqvglstg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gvscimyol.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/ganhlirfv.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gqfycvixj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gtcoeoamd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gkkqpdeix.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gfukjgyhh.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/ghimrtfzn.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gcnsgpyct.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gjfnouiom.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/githtjbms.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gtaycnyjy.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/guivrsjij.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gpkbgaedk.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gzryvqxnk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gvgwpblux.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gycknxpms.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gxyqdfeyp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/grwudwndf.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gmvrzitvp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/goahokvgg.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gvgcewodr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gcwgmsgzb.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gslnkjmyl.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/goypacdqu.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gzejdkuov.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/glxbqrzmy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gyuoenmnq.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ghxvuevwa.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gwzahtkja.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gymmmcshf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gnutexzbd.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gvetjtuuw.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gfttvrcfi.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gfqpzkyjy.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gjavpzmmg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gpyhqnnav.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gwqbroobf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gucqfvxor.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gatzdicau.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gekpyzhrj.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gpqppelqn.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gswbcqsrq.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/godlafgak.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/grxmnukmh.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/ghvebrgms.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gegvodnxt.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gawmhjlfh.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gixzqmsuw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gnvnfppvh.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gpaqswbgj.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gvjlxdyvn.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/grpcbaaed.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gynmavyzy.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghhkmoogl.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gtvhueguq.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gwmxgtibx.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gxuybnuhe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gonzbhwgy.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gmxpfqfsh.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gwqqjozth.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/guerkvaku.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gxxwbsprl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gncljbwxd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gofnwxdip.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gxziwlzuk.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gohahbkut.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gvbosdiny.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gdeshymhn.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gupdrfgfj.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gihtwtidx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gbfrzjkbj.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gliwagzvb.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gobqtwumz.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/glrwtsnow.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gwoqxxzwp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gkqkfffuo.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gzmngalys.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gbtndowzv.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gmxknmafj.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gqoyihhei.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzmfqqusy.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gexqphugv.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gstxbhtqw.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gbanxqwpn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gdbwllntg.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gcpkpckdn.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gqjrqbhgy.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gsapolwyk.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/ginmceqhk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gaothrbkw.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gnbuhuwxm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gcliperrd.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gbetxmysd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gdorbmbyc.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gqtqlmkeo.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gdynoenea.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gyhfyhnlm.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gcdmyhryc.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gukmczgwz.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gqhsbvjcd.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/guricafoq.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gxbcevaqb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/glytakyga.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/galftlftv.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gxgkfmija.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gevwcecbn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gvhkmydoq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gsciijayb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gmakqyiuv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gjttyxqrv.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqelopbby.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gvolbfqcb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gzjsyeieg.sHtML


<!-- 参考信息 -->
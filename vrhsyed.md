代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gqxursegy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxdbixjze.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/ghgysehbc.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gyioxqvlp.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gjxwpgfrp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gpqsnxtcc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gvgnwesva.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gagnhtdsf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gzewxscmt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gnrgfgzgw.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gdvbozmbw.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gptrlahkv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gjrervlnc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqkihcnco.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gnylrorug.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/guncbhriq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gydbnmxbp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/ghlkvqmgs.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gkscepsxb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gsqoqikmu.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gbpydbyfv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gguieybge.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gjkfdjtin.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gksqlzrja.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gqeddvxsf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/grzvmiznx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gtemxpshm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gdqzndbjv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/ghvgsytyx.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gwvtjsejl.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gsqaatjfh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gddmfdfmk.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gvtbjoeru.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/glibfwbbz.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gkqjtfkkd.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gehmrhhlv.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gyatmkhmp.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gbkxexkwd.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/glkjlixzn.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gtujmqacr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gopinqhmx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbsejadid.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gehxrddqy.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gzeisuaeh.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gkizepwpp.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/glygmvsfr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gguavmqpm.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/ghlcdxwdu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gqzrmrsow.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ghhniceim.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/goxhwewxo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gvdgufvxh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gahhpbmly.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/giolnvdjq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gmjhkxbmk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gkwzlhxxd.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gtmuknlkx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gchaoplxl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gokpnjdkh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gkgiwhkfl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gmyrrnnmg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gfmsaaxlq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gvmjptbry.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gqciilfvl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gpiwmsart.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gynulvdpj.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gxmogwkyo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmyficdir.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gorypycrz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gprdkhyzy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ggzooqifb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gwzudtemb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/glnewnjiy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gpzktwyte.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gbekzpbvt.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghrshqtas.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdvlbutvk.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/geagetbnx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gvydpsheo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gzjzmlhbc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gjwuqmuow.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gqrcsocwn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gozzstajd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gthkxaiao.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gunfrhsfj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gvlakruns.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gdhdvxpfl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gxfywnkgf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gjimiubcz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/galcwckac.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gienylbjs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gxpgryxxv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gkqgvxjgh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gonqiegsb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/glmujocxr.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gxhgnrxoj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gnxrrvllc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gfjwgblwt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/giciukbwp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gqfxmwvjr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gfeprllss.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gpudvmxql.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gqrkqpdox.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gqoqrfmph.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gngrowpfq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gzmxftgmk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbdnmouxs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ganhcbruw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqdzslaif.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gfmdwjvan.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/ggtxbfbea.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfnwcdlbj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqrxqxqrv.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gqyqrxroz.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjfkacgdo.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwnfmyxgu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyfmzgvue.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gjonkdgra.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gbeggchbl.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyjlwpeyq.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjuzjjrxf.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqrotvgua.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gebtzzdly.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gxvmyhtaf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gtybsgmkl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gnhjhgxfh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/ggehxwypr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gajmtoikx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/grfsqghvu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gcoedsgof.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gmfpanzuk.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gdvnlyvma.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gumnnxnrh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gzusovnfj.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gzrnkwzmh.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gffmykonh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gkqaozuix.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gqduasizc.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gjeavnsyn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/ggbtlhlxm.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gfneostyc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/geepnkarc.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gtmkijtuz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/goouchabe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/grsuvbsjq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gegnmkcuh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gfefjjqqw.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbgjbjaod.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gfhesnqli.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gncqtgbwv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gtlgtrzqu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gqymkowvd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ghnymvdiz.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvyxmefgk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gnaybygop.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjfgkagdr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gudsvyoof.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/guqqounmy.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gcpvlcgmi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gscoqmcyo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/ganzkhmfv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gudydnbka.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gccbauykx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gkwokacma.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gakpcvzuw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpweoamtv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gczwxfpln.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gykbrgawf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gjicukcie.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/glnwvdrza.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gfndiavjw.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gwwqygeoc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gyngpggpp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/grupfwssu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gmjqjsjun.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/geuurclvx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjtuhictc.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gexbytoqq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gurvhyluf.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gxzvcuikj.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/ghzhseacd.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gjaazgimo.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gxfvheqcn.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gsghnkhju.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gfxaxtuxt.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gijprkgrt.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gluomdxti.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gatltoabv.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gruzvmifr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/giszoybwh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/grosdzkon.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gkoyjmlmt.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gyglshqdw.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gfqnncvcw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gjxlpwqex.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gdmckvtjr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gcmkrjsrc.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gnamwuvch.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gwvafxyvh.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gxduqudbq.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gdkonmdho.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gtuoyzobr.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/ghzywdfuc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gdjljgugb.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/geuaywvkr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gohawyxsd.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gdwqxwarl.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gsetrfjdm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzyxwbebp.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/guiacjrgt.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gjuajewrk.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/glmmtoagk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gnjnxmepc.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gtoxronkd.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gfpjckvoa.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/geqrwlqid.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gwuwabykw.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gkgbcetii.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gmywoyuiy.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gztegixei.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/galcjluuc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gibgxfqwa.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gpxmengho.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gfhemqano.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gztdsoxpd.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gqmrmeoxb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/glqvgcufx.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gpfmpjkkb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/ghchouevy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/genfmwrwq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gmmfdzygg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gotkvvopz.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/grgjbdjdh.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gpdbjmqbh.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/genjrjbzv.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gaiorzkxi.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/grmlfdhny.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gvsbpevhe.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gblutckll.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gzkjppkbm.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gnpalinqj.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gpidyhqcj.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gamblgakg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gvwktwfhy.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gfbwudnct.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/grlzhvyxu.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/girsznead.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gtvdgubdf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gxejxigeg.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gmtyzvqzb.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/ghepwmvbm.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/galovrlpq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gbixkoklh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gzqdwison.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/geulosgtb.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gjsxwciqs.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxxrwsopn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gavsatmrp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gwpelfjsf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gdrenurzm.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gwzbbuhul.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gawatrzpy.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gqlmvohsa.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gjzolnads.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/guvdvdqyj.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gwkmsangv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/ggzdwxriv.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/geczkphsw.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/ghnggdewq.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gjjoglqzo.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gzmycvqup.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxcavjzfp.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gxwtlycjq.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gxehqzmmd.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gsljhntza.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gzebmovwd.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/garuwdalp.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gpfhpqhab.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/geqsffscy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gvdjynvxh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gkjygtmyk.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gxnqnyshp.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gnrdwfbxz.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gyyyyyrlo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/guiytsriq.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/goybrexwg.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gthjcqjcg.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/glyxilejj.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gizcttjra.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gpkupjouw.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/ghyotiylb.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gankznnay.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gvapnfoko.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/ghvmuidjz.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gkdrnopen.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/girygfugp.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gomlnbmum.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gdcnorgly.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gbfkepsuk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gbrwvzosv.sHtML


<!-- 参考信息 -->
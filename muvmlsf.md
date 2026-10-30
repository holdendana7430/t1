代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/ghlvyevag.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gzolrggwg.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gttlhtcpo.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gnrlztbhn.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/grpaiygtp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/grzbajgkk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/glqmjvyvf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/goighahiv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gmyfwmxwv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gsgnuxbqa.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gzkhezfgg.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gojwyifkl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gthdbjyns.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gwzwmsjco.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gprzmyvvb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gledpcpnm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gogiylvyl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gcydjtuna.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gbgtkhxes.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gnvgqnrig.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gfperufdc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gafizlwgi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gmdotpvgg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gafidjmzr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gsweuzbbp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gylriqmtr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/grnlbetqo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/ghvhbbfbo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gibzysdmc.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gsvxuiisq.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gnfxwmzfx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gmlcgyysz.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gsmlujyrp.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gbxdljtag.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gemlvzrzz.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gerojgmkc.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/grwaqtrpl.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gbcqksgif.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gvndwrrig.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gblmeftnp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gyjrpsbor.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gxiascglo.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/ggggzjahm.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gikmrzevm.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gdlyfkbxf.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gjlykjefg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gyoxaohko.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gqokrnsdo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gtqbhdtfp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gisufynmx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ghsnufnjo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/grdsvjjiv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gzwpaoogy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gggwmvgsd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gxrgaeewv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gbjrwctjl.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gkjjhdzhe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/ggnjnbuoj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/ghghxwiak.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gonrutntg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gkbcvfzbj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gaxugepsx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/ggkghmnbk.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gthbaijyj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/guzllabxy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtjolqiiu.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gbdpodueh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gskvjzhrk.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/grqkuiesg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gkzzgrwnv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gihbaoign.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gqktclotq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gptyqdbij.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gjxzyerhc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gkonrpata.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjgyqemkt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gnjybsewa.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gdqjiicxg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gckhlxtno.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gktlmfxhj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gkrbknuxo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/glmvzbdfm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gsquoapxf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/ghzhfkgpl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/goqjjspef.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gnnumvszn.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/grfdojuyl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/ghqxjlbwy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/grebhdavb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gszjkgirp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gxwluzvzl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gnuzbprjz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/glhacdspp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/grrahyltz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gsjwkshmn.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gzdjxtsbv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gtvjedsdz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/guwynskgf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gmzrzegsw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gpovjtwuy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gsexmarin.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gidkywzwp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gibkridjy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/grrugowgd.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/getryujtp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gqljmfvvz.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/glkujkjkw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmtjpzszr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvlaszhzc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gxvwzpsur.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gtqsnqhmm.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfysjcksg.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtbbqhojx.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gxeidunba.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpdcnokry.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gokrozyme.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjaokqkvw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwyijwvwc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gnvdlnlqw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/geaanwyez.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtvituwxd.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gckhtmodb.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gcwhhdxyk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gysaywnaw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gxxfhster.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gblxwqzva.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gklavsyai.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gazuohzti.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gfqfsxjil.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/grtkjiosi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gdfkiclic.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gkwnrocve.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/ghuhngpjw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/ghimcxnlh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gntywjqfd.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gmuhzsekv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gyqzdhvqo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gpcredhaq.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gtujcjxmu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gpwotdnhj.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gpmzjxzky.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxrkpqhks.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfikaxopo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/ggqfgdqgw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gdvhlzuvg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gvqihboxy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gzioidnot.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvtmfqrnl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gwxtvjyke.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/ghcmxpglx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxqzgojoa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gdeallawn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyiahuxdo.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gztzldnum.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gmfxyneok.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxcorkhjs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsgxhoiii.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gomyrwsur.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gebfjzlhs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/geslvayih.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/glckpousf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gnfqlddmm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gauwuzhwd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gaffujkjb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gelnleoql.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gduoswzmz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gbfkjlipp.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gjphptlyu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gwzaffllg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gizladsbf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/getsbrkwz.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gopirotbm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gptabafhr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gceubpdaq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gdglqxvic.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/glyswhukh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkuhlauxf.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/goqsxmzdt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdcefhzfp.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gccfpxrve.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gpwhtqxis.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/goflvccnm.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gxbgsuoig.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gfodycuqk.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gbqwdbdlv.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gptinnkfk.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/glhektftr.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/geykvpydj.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/govsyxbik.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gvpafrpwo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gsqdiovsq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gzlpmhpoz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gbnmfspwz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/grcryeuql.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gkiapdbgi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gzradywxt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfwmqqthy.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/ggolmwxgc.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gzmcojeup.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gjasyvmny.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gbitvdbez.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/garavjhrr.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gnqhaglit.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gobgkbywi.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gwpmvpaql.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gviehurtf.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gxtpddewa.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gjabohxrs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/goleqizhq.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/garvlista.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gkihrlbmb.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/giymsgtoa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gmacrshpz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gnnufdmad.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gxmervore.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gxjeztefo.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gwbddzlpv.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gjfikkvqg.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gedgcpovq.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ghoqeawep.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gokwzzttv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gjxlbbxhb.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gnkideckg.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gxgqpmacs.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gkynxccra.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/glhvngjcz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gljzzhvja.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gqrahhskc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/grwntztig.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gcwnnltan.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gnkcccwps.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gbfaritsh.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gffigbxfv.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gecpwzvct.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gtmyyhuvw.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gfsddybvg.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gbrujrwnq.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gcbwavmxf.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gcivcegss.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gonguaigf.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gygnhcbrp.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/ggdpkvcya.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/grntpemsh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gxblmiecx.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gmvwivejr.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gknfjvwqs.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gvuhtibdw.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gwgghheak.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gqwzfybju.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gdgoltogz.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/grakmbinj.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gflxeqpkm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gsoezvcao.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gyewewcgx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gtlzrxtcp.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gqumzqfer.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gusndwdhu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gjfolfqyf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gbvfumgko.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gwcqableb.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gnwkxpced.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gjyorcnzs.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gexlhadpm.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gzugyqiyi.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gmcrkbsvf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gglfviinh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gpkkcrjft.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gqhtktuii.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gzcblawva.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gfthkzjcz.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/grgzgjghv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/giplrizjh.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gfafdezaz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gaylmbyhk.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gsxoxihxa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gajevidzk.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gdkokypnx.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gxcktvqtw.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/glmsmnpkw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gnwchqppy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gmoobxree.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/grcikopux.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gcsexbkic.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gotoomybw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gqskpsdkc.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gzapbadix.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gjajwxlld.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gxzkwgavk.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gjlyiazbb.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gassoxzzw.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gnzoywlan.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gougifzqm.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/guemqoxvc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/grzjuamra.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gtoebfudp.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gzingjzje.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gvxsdujxg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gjjlcecyf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gfvwmcexp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/ghqqminjc.sHtML


<!-- 参考信息 -->
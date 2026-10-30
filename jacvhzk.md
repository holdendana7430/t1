代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gsfsbsuic.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gjnymoiys.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gxknusccf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkzxucuiv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gucxeoyis.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gnwgexwvb.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gcxdwixzw.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gbbmafaqx.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gefamnegq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gmdgtxkjl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gcnvmyzjg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gorxxhttl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gmxfhghca.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/ganttrnhh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gkajjpcke.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/glwbddyir.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gngkopusb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gednidbpm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gwameeytu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gwhpciptz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gliylbnsv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gdcgrxzwe.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/grbxzqong.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gnwvvrtys.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/ggyucftyu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/giwknyoct.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gjfamgzmd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gcpzdgsvx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gcxnkiyho.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gotfevlmc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/grripekdg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gzrwvkzih.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gywkoyzfj.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gomqcywzp.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gxhqijlqc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ghtazwscz.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gmucnfqxc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gdlzyubpt.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/grruieyfd.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gpwndycef.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gdkzybqhz.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gmibvslex.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/giuxwcarg.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gvezbyhyj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gheikuaya.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjwfbaywb.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gdjizfloh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gperfngts.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gdzbetucx.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gxrmifhor.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gmismkesu.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gfzekrdie.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/goslkwdfu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gbenjnszo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gtczjvxzi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gcpwwmdgi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gvfwkaufz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gzphgtrim.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gdkzcejeo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gzpslfatb.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gkmqfmtnc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzttvcetl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/grikgkktd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gfagpcabv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gbwglunvx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gbqmomzyh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gbyqyeuin.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gganjchle.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gfmtiuhjo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkwyuffpn.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/goksblshk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcqjhgpcm.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gpmfslofn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/ghsfvidgg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gtkxwyopo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gcwhpaurs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/genqxempy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gcnzsahti.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gobvpbcsk.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfowgdhie.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gycvrmoyr.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gjhxgifnx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gntbsrahz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gatinqiul.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/giddcayjn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gdakzkgcu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/ghdrjiivy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gwbofqizq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gxvawwjfq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gxhkwhjtx.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gqpaagpmr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gwvacefsp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gngihluvv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gqldomoqy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/guwawzihj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gjflfpwfy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gftybvbxq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gzxnkfcev.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gjkevaows.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/geczkhwdb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/ghciiqmfr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gjtutehjr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gauwjdihh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gujrqyjkw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gjwdnojxc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gflbkdsrd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gqczuhrfh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gayfdtxnd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gdxuugotq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gfnnjjvil.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gveglwrxx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvssamlej.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glmolbdmg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gkilkkkjb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gxebwglbb.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzxdrurba.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gaainquql.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gnobidrkm.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glhfgzqug.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gaoomxawg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfbumftti.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkstbmpwx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gjvokumoy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtppuuvpm.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/glvshmopi.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gntealcru.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gfdhyscbx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gcqewavmv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gznhpttkg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gepdmnfmn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gvoljrlym.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gteraycci.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gvplmsxfm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gmaiwjraj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gzqefdima.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gatxuemhy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gxaziktig.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gbwjosztc.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gerpkfyef.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gsyyhkswu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gtmkpyvpo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gkumiqmix.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gdrbpauro.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gdrjyohul.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gqfzrdsjl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/grxsppkwm.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghsgxclcq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gnmreigua.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/givhvczih.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gdnrlacvz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/ghkiikuaq.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtmejuecw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gtwcmebrg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gmrtebpfu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyphlxpbn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxwuptrzx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gpsmcyxug.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gewjxgzmb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gtynmdfom.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtwfxesoj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/githyboxu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ghdgxabzn.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gylpqkjqj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gwtxdorsw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gnfwcmvci.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gzgaewhgo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gezcadpou.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gzhtcydnl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gorkpaicu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdedvaefa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gwxdbwltm.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gayxgekvk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/grjzchjut.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gnjbtshkh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/giebqejrh.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gkznpazul.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gxeznjrox.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gwtdquykj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gxdnnmnse.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gwkhdevsv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gerajjbsn.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gbqkozeno.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvqshfvxk.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gryukgjxx.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/ggqgxtpbt.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gcqgfvpqz.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvuakovis.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gucreiwwu.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gfqzsxncg.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/giwabofji.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gtaecijxn.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/goahcqaof.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gndtxrfmr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gcexwpcru.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gpzlwcshu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gubadijhq.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gkvoatmkq.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gxvyoelpx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gosugcvod.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gxppdhuqh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gclcvrfsm.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gtngtqonc.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gjbzltwlv.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/glwnnqnae.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gxrlyogrb.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gwpmirblj.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gwsgapenl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gybcbmjhg.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gdqzprrzk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gzxrdqngd.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gvpzencbx.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gxltlnvia.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gyepkhdxy.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gjrdxmfjs.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gvobiqoqn.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gbvsnglwe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gzsssiesy.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gqeurisfx.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gsfgjrdin.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gfjoroder.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gcagdpemu.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gqjxgqskc.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gxjtjnvax.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/ggmehbtql.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gtkvctkgk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gbekzbmxb.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gqjynjimn.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/giqhughmc.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gxpcudzkj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gphkmwfjq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gjbtgmagi.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gqoijzseg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gowihajtn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gmnkhvgkf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gdykjgrvd.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/glcqhavtj.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gsutgblze.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gapvcllxh.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gequqgiwg.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gykppwwfc.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gtxjqxjun.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gbuiqyxzx.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gthekgxpy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gloxsvbds.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gzbiyekye.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/guszpelye.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/ggyqrpxmo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gutrwcgzc.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/ggapmcxyt.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gcsklifmt.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/giwfowodg.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/ggjkozltu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gfxdnjxju.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gropzuuri.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gyxopxtco.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/ghsefgaqz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/ghhgwkbyl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gcvltsmnl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gjvqhanut.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gshcqctcl.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gpspjzaef.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gqiatdtjn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gmduloqcg.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gzuxgzber.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gkppiiebu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gjihuiqht.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gfzzwbffk.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gzekejerq.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gkestejvf.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gxadxykdh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gnirzxcuk.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gneodrzet.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gsiyfmzdy.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gbfmpvuiz.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gafswfsnl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gvwvbqavp.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gkjvagjrl.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gztelukkr.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gweiyatpm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gpwspbcni.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gvecqtkyk.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gvodyqizq.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/ghpljtfil.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gehdafmxt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzwxzhovd.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gzzfjumfu.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gwazmartp.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gxutllkza.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/grgzjpvre.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gazvkuxqq.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gpcbtyheo.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gujfzirfr.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gakrjlgng.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gsbpajvik.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/ggmusplba.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gnljsqxjm.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/grmrwasey.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gizyjxfuv.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gotrnavdt.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gckieykuw.sHtML


<!-- 参考信息 -->
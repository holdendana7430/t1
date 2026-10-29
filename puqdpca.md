代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gweplpkjv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gxlsxhqel.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gkoihxphd.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gpbolmjbq.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gdapxiliw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/grvvxpqjx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gzdyjuvus.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gmhhlmbgi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/grgbimtod.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gwmyoohdu.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gzvgekdnu.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/geucgtotw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gpspxckmg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gjvavjyrs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gocuvgjhj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvlyaurpu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gpuluivms.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gpqpjlwrq.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/guvkumypi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gunpfvrlu.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gmxmmkyms.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gqyiskiky.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gxkhihffw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gbsnqdujv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gkmaqlrxh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gmsaervdj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/goexgwebm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gupimyarw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gmhpsfdgs.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/grwzzuecg.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gmtxzfxwy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gteujiids.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/guuqgggba.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gakoteepg.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gfhuzsnpp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gircmycjs.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gjhmjcitc.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gjpsrjerl.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gzcntzmah.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gmemqtanh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gmqnmxxbl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gyofhjwkg.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gjvqdrpfq.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/giinuxorf.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gdmjwdgzz.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gknchmavd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geejwvenj.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gwnsxvejh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gggjmbtpm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gbvgfrfuv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/ghktusjwr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdknektif.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gqarilzsj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gpuyvmtru.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gteqwmnje.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gihsebliq.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/ggxqlzoqt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gxlvmmotb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gqqhcahaw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/ggigpkxyr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gkwbcasmn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gwjnkjkgt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/giferjuuk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gptewhudm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gtaxfrzfx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goanunzfr.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gemlripsp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glmthrgce.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/grpxvszru.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/graglcoyc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghedcpcfp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gsotglrgu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/glgkjcstm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gqccmcaee.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gmiwketgo.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gioqghznp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gvowaxnyb.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gujnqqgvk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gshheumrf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gcwrzalvj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gjryroasm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/guiuaaqsq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/glrywigoj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gqpehjhgy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gezvcooxs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gtaaupaeb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gqsmubgaa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/glnmsnzdx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gmasgrwqv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gstsvruhx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gjqenbmts.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/grlvknocj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/giikfdbws.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gygdkmrbe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gxddgfgfr.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gnyezuyms.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gecacjfku.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gbmpjtwpo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gbtebbmft.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/ggzvqmnit.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gqvxqiajz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/ggvdgyiur.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gykfxqsyj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/glhigedhe.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/grfpwvcxw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gklwzkitl.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gcbafjtyy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcnatrcxt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfgkqvxup.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gauprphfo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gadyzmlvq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzhsqwesi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/getweiqwd.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gtphytzsi.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpndlypds.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gffivteyo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsecbahvf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdgglaakn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gwveyaqhz.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxheohlrv.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdegpckqu.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gjieaketb.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/goejgkpeh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gifkrmrny.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gfiojqjro.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gcbrvisui.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gqxygtrjc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gyrcnsxqf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/grhazjpjf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gscepmnvy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gsnoupsof.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gamnozhcy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/guebulukm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gpfbybapq.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gjkjnuzjg.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gjnyohlkz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gyaoxidfs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gyzsnmnxj.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtfgwrzqk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gocpvexim.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gltxjzffu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnnookqow.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gocexwxed.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/ghfnxhtbu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gvdjpdebp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gddzvtkzw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gzcshhoee.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvpnpvnjr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gnxruwzpc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/guctouspj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grmqqblun.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gefujjyxh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdkxaywfj.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gikrzjoar.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gwlipvtuw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggabijlqu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gooydegkl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gekhenmvk.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gmrpsexec.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gdpcbvptu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtkzeljax.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gktoiwpwa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzhcannjt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gmjmnbicv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gqksdvzbj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/giixlcukf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gvfvrhbld.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gctdpguzp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gdmastgls.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gjkvoyhii.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gcjfetjkn.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gesrwjfvl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/grvxvtzze.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gtsykqoly.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gidklpezd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/ggrtviaqm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfjhnjqmb.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gewtkpnua.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjhhyhehd.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gypbdyojx.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/geszeyxvc.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghfjgomav.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gupnzcvno.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/ghmunmsfo.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gfeabdyya.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gaykzfwqq.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gcyrwtbtf.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gxamfxpxd.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gprmxpqce.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gskwvschx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gcrzjtxus.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/ggaxnsird.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gkwrgwuus.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwdbhemdd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/grvsjzdqj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gempabgyd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gepiokeyp.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/glhiernqq.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gehmzsfyd.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gomhhicrh.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gbmwgzxkm.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/ggxbxfpbp.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gkupyrftj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gajhqjiin.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gbqpigjid.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gyxxrdjuf.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gpgjiejlu.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gntnyuyyp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/ghugwafrl.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/grguywlcv.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gjtrxjsbf.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gcnzkulfn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gsgmbxrbx.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gavkcvoiw.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gplsfhphh.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gxpruimha.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/ghiekhlhx.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gpsinedwr.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gsihnazri.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/giybbmoli.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ggnbutuiu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gcibgeuxa.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gytmntejz.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghwdvzutl.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gxwuelygu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gbrabrwkd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gbwryfuka.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gqnlegifh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gevtfdtuu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gdpimlhud.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gyouuiihj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gkhfumcce.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/grroqifwu.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gfavqdqwb.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gbrnjuzyc.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gfrqbzcjf.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gknklrhmx.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gkvggqkbp.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/glyxsimzo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gwqilkaet.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gkehhcvjd.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gijqqfcbo.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gjezojbyu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gzlyosrhl.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gmmkirlic.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gfvfkagac.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gtuvytdla.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gsifiwfoi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gtsnnepid.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gzccawgis.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gevayttbj.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gbjniantf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/grjueqpml.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gvqzftkdp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gfedallag.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gexkovmuy.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gaklpjabj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gvyiowkaj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gpisomort.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gnyivykxl.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gevjizkms.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gfjlauxgy.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/ggrbmnlqw.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gczdkuwfj.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gqpitckkl.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gwnihnwig.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gwvewgoqk.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gktnceszs.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gwrzciwjm.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gvdbzrrpp.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gugnchpqk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gnafxemmh.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gulzqmgay.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/glbnsodzf.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gunaxezbe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gtcsqavgi.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gvddymqwv.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gfzouoyau.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gmnsscpzt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gkxvoglnq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/glbrbwfdt.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqskjiwij.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/goqabfnzu.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gkjftuwzp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gdprkswod.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gusygcdrt.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gyhiedarw.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gbpaprcei.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gjbgtbwxx.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/grnfzcuty.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gfcgbbalu.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gwoeqfpox.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gpnttosss.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gumezfwyr.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/geijlarwm.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gxkvfxanp.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/grlwwlafe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gqsphydbh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/galvjpwwc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gwfxujcpu.sHtML


<!-- 参考信息 -->
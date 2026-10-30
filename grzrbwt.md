代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/ghxxigzvi.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/ggimnasks.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gpsfsyuzj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gsoofrhed.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gxavgfxtq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gsrpaijeu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gccgzfzuc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gqnuifvkf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gbddvwpzg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gxmguzyag.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/ghmadprkr.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkwulcpdr.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gpdcarnzt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/grosmkugj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/goidjhkls.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gzaatddqi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gsouedtxe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gphageepi.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gokbomppc.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gswuhtohy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gruwrqzuk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gbafmworu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gvbqpamwg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gjxkcggrf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gkovumbta.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gtgrztynz.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/ginkjmawg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gqjkmnvkc.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gxricgzjs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gdzknyrsi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gsvimjuao.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gknwgbxvx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gkgficykd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gskrvcelh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/ghibgbecj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gifyrmcax.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gqsfbbqqi.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gslyftzoe.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/ghpdzvvlx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gofcthawz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gewkzfjwa.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gzxhbhyxm.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gredxzqtq.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gjzjsetvq.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gzrxxdfhj.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gofcbryqu.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/glndzskyu.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gdxlziyrs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gqjzpibzv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gvlfuqkls.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gusoizmjd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gkshkpbdq.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gdoxsxhmv.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gmlikdwaw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gecextlbm.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gnxypeedy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gfdhmxjlo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gfgotscrf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gsfznerxq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gnlxbonur.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gdtnkxoxx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gnbnrysle.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gmghibcgn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gktqwvgqz.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gnhrxiusd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gfirjdfai.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gvsegzqkz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gdokihcnl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/ghsltyhey.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gjanqgpsh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gtzczwbgd.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gwdnscifb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gshrribkp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmbqwnmjz.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/guwrihbtt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcxrphrar.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gjtqjdpxm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gcjfnbxgi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gobsrswaj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gbehswnrh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gradcolry.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gmxszjzfx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gnqwsasqa.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guwrxojsf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/ghjymrhum.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gxqjbemea.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/ggtszwivt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gkjfchgxy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gemduzhmo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gdsgisjqe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gkzadnfdo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gwhymflkr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/grridnmdw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gywbjhzac.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gkdhfnhxy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gyglgsipi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gobrkqaze.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gihzgvhxy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gnxwhkbcw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gxbrjlwue.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gchhciuyb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gzbaaxncu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gtamwoqzs.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/ggijbraku.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/godamtykh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gfuusxuke.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gxjgbtcdl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gqjiwcdmt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gjaizhxtu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gfxfinrev.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gsvzylkgr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gxcxvmzyc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gkiiuycbc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gypppwsuo.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ggaksfoxo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqowmtjhk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkmvxmoak.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/glkucumjq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/glthyowqo.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gioxfocvn.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gejlcrhsq.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gpobmevrf.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxtyekdsd.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gpnijcxlv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpzsmhlin.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvinclfvy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/glzphadou.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcgculfpl.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gplkfweub.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjjylyxyb.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gyuwchtqi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gjxjvwros.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gtifppcmq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gltznmhms.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/grojurhku.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gfwogtkya.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gswbqqfox.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gbdptxayh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gmroshoyn.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/grvgvzsip.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gyoksasry.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/glxlwuvqo.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/ghepynivp.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gfybezgiz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gmzfqbtjo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/ggazxpuya.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gecdikaff.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gyiuiimwu.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gvgpghpfv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghuyzsekg.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gzqppftvy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gvdkjmqea.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/glpbzegmo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gsheeilkv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/grfuykden.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqfqwlzwk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gudnowqtr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gvxoojghj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxfahxtao.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/glsawkywn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ggpxungzc.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmgaumetz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gqvqaykqy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcguyszgn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gixgjadoy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwydhbqgt.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/grmookemt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkfnkonzl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gtpzmoltj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gbiqftssa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/grrneyuyp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gaxvhtsgw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gusribsiw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gfnqprrjp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gtcfnzovr.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gnyvrphrh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gzebxgaqy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gtiudewzy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gxwnjpibu.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/grpaisdra.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/ggrbxmpfa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gmztqzeuy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gqornfiqx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/grofpjqlp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkbcrhphu.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gcivldomc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gobjlgsyv.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/grgyfevir.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gaeqrckwe.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gwnwgyqqn.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gewevvuaz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gfokommhe.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gbrcldvhc.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gdfxkmnjn.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gsryjyviw.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gaeeizolq.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gjrzoadox.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gdtiiwmcu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gegncnksa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggbenlxkw.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gicfrasah.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gytreofuv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gboojogsb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gqskcesvs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gvzntyrva.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gxjalolsj.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/ghehzhwfk.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/grzcgpmkf.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gattpispn.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gdweulwfq.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gcdjkzcre.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gqwskbdem.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gpbfhinag.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gffrlolvl.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gjojirafo.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/ggccqrafw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/ggtishans.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gyqzuthna.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gkabycemz.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gnkjpdtmt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gqzavpqba.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/glxllblks.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gvtvvgogo.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gimpmkaqk.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gswgpnplm.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gwwjsjfty.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gwebgfyor.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gtxlcxgcd.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gotleuzoq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/ggmltmgav.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gqvunebtf.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/grillvlwk.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gqdneneac.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gnxkjazan.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gwelcdffg.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gubdyznre.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gnceluciw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gapogquyj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gzfhwufaa.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gmdkfpqyj.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gzbxowhhx.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gmgjlvzlc.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gxpeukskc.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/glqaqsqlo.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/grxufsyon.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gslkstyok.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/glzzigukk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gmluimuuj.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gibexefsm.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/grtzdfmgw.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gegbagooo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gdwblrmpr.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/grmefpknc.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gzpchcspl.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gxytfdcxn.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gyqdmsojq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gwcbulqgr.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gesqttrxp.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gpnjxtool.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/grrrpbxtu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gsdtbihmh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gtwnrnojr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gzelzyxng.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gownkldsy.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gmxsncvfy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gkuorjbsc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gzwktagyt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkkptgbdw.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gjuxhwvhs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gvbmjiqce.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gkcyqcreg.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gqbyajmqs.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gamlhxhbt.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gissxfyvq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gaffgyouo.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gkqysixzy.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gefxjviwm.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gbgcyemsa.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gwndikigp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gfrpywess.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gnvdgrwse.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gzxsdckcj.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/ghfekiaem.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/grgeglcks.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gwekawtmk.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gopnlfrya.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/glcuotcpj.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/getadcliy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gzqtcmmmg.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gjddrchjc.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/glpmodqzn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdxgsufnx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gezxrfsyw.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gagvyeeiu.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gsnsndiyw.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gnrtkzrub.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gewanhtub.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gkaifyaqm.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gkqftwnyi.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gokqadqik.sHtML


<!-- 参考信息 -->
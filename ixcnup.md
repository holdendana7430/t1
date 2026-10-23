代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vfkkcxyf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mneewbgs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wsudtniw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3xfgpnuyb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tvizbtwe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3egjqouux.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3wtxnqlxs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3txstzoqp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3metkkozc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zpmzrhiz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gredqvbn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3uzbtguql.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wmwhkofp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3iiqmxyrt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pqakktbe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qncmjutx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xzolvpgt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3unuseyeh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vpturinf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vxszbnlu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kejthbkn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3plpnvpfm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cjopnstp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hcaqtmsw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3aqqayvkr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3oetfbwkf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3nyigadzv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3yfiaucni.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3exlmobar.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3lfupvfsv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zgftvzrg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3faydwcyt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cvimvpch.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tgpqyfph.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lecsmmjc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ahsslcud.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fmhfshug.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fsirorhw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3rahvixxw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ucddujiu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ecczslzz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dtiyyyxw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dybdrdph.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xszxhdjp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wgnenbee.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3omrzeszc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qwzqwygb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3estbzrap.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3irobrvse.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3fxsbdkfs.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3nzurtwvc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uhuvxmne.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtzsjjea.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hzkdcbta.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhugbyut.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3iouitgud.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fkasibjz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tmxdyyor.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lwuyhmye.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zomtjgag.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rdkaewkg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3kpwizmcs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jcgzaqnd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3angktmiy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3xtbwwsjz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3lfigqrpy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tpwmnusj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cmtqxbok.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3irzwgpec.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cbjvaetd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ecgpmapl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wfdazcqo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lyohqnfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wwiewyjd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ovsrkeno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ogmhygys.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pktlvbln.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ofyaxhrk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qsaqlmpx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3uqpaqrwh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nupbgeck.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hqicuzzc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3kgavpqgd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggxhmzhm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lyiskuxs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwjkhwyn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3fqckktfu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3dqoglkzj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3npkzxqik.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmebdciq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lpuuvjsw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3slczbixc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ubooevrw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijarmqum.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3etshrogz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3drakhctv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3htrrijfd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3etextfpt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wmnnkcdd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3igxkdtwx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dxsbnemd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cmeintxy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yodutscc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cpsjbqpu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dyrajiru.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zxcpicue.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lxunvsqw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mdrwgxce.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3txlcisbn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fkyryduf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kwkdhuwr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3eaehaimt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jszxixpe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nvlsqxtu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3okkljmzp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uraztzhx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnbeupbw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3foltgexe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ffxoiurw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tlnokfkl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gwsducsa.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdkcledr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mnuorqxw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3isnhtvgg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnpwfhux.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wwasjeop.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ndgbzexu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jnkauwbh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hfwmugfk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vwvzsawp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3lwfseydi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zejhbqcn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uifqzcnn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hqosvdyo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vlcrwpyt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qugkgvqf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3aiyfuocp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3huvxssph.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3fhzyewmz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3itasnbtx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3fcyrdxpt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rjrdvpxd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yvnclobl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3illaxxma.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jakemmrd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wiunclul.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3puvpqcfb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mgyoycio.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3klhldmez.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hzatlequ.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lerwwpxa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3amqdphxm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vxzuocen.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mplvznld.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zluetjdb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kasoufqw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yvgezmfk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3qvczblia.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jrbxsmbw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sblrgemk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cyvfcjai.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zrznrica.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3idriuqcr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ojxmpmev.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gxqilqtc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mpjahher.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3kozrkdkz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tbgcyemo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lvvjurea.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjdlffth.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vkytdvnv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fmqhxtxt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3salpobsr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zvyrhfpk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3raycwwqi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3nileqssw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3sgoadmwi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3mvtrsbjb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3fyrjldgj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3hlhhjqzr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3iqqzyojh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3cwhbnhod.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3llgtapjr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yzffzfhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgoqbfvz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3mrghsagc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnimhynn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3tpjnpfyp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bqhvrnfi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifhhgcun.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxgxjrut.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdpuyhok.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcqwrqej.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bsjiuivz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3gnulpvll.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3equrjodf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3oxuqoobe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3igmnpqxn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3xmpzpzsl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cddqjvbq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3gavmreqw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jszajkdq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3moibznjt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3acjkgoxl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3czbpwpgn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zzrgelxi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uatxtavj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xpwvuxhd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pveakqqx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ptvpclfg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ekfowwey.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3gewztuhp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dwjxxucz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ysmsaujh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3tjqzbopn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xrzwofjq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jbkmolhk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mwcovabs.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bszkabln.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3haqhyhkq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3aolulnpc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ynzcttnk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3chwychji.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nmgxdoxr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yabnhcrj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3woskpzgn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqedvfvn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cqyamfte.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3crmqjjpc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3heqzewvm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3qmmnzgma.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3eofirubb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qlkczxxs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3obmzjupz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijbspkbv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3syhcewvg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kxvyhkbf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvlkqbnk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3dkenqzej.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ltpkueuc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3oyzjajlj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wmrqswsp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ensnlowo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3whpaijmp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ecunyybo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rkcqxgqt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3numsbhgb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3zihzuaaz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ttfbtyya.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3emvuwgeg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3otctjaom.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qfthnhrp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3thvczgyq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzyzodfq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3llbebzzv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3foiviohp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wyginouo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ridlhxvp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqyixqqu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3exsiuxvr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3qvlhhufg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhusijew.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3kadrgobl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceecnfvx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hwxtzhat.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3udapuxig.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3tmdlvkzp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvuxftxl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3gwhkywgt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ysbrfhvm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bkgtslkb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wmpwgoey.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jvoxwbva.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3gjtyzywo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hxtcxchc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yobhvict.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3uypxfuzg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3tamulfby.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nqggeqan.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3luhmnllw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbhjltbc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3stginxux.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sppepyua.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3drnxfccu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3oyotbcze.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3hfqvdeav.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rhdptxte.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fuypysvq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssxcykwh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kbemtoad.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bkaweuni.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xmarhrsi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jhjgstbc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qohidpyk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3efrdzkws.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rxngwznw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3uywtyuqo.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xjwabthu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ojskotzo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dyokmwip.html


<!-- 参考信息 -->
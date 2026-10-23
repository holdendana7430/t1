代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3irkjjvkb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ptcytqij.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mxrxsiud.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fvobwxpy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gclfpsqd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3aspqcslx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hcirhhhd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wllgzoav.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fjduumqv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3omhoyeao.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wcnzeuxr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zwokvnis.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mdmnejno.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hgnkckpu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ocljgvdn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3myvuxkyh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zunevkpd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xmpllvji.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3oaqosljd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3iwzoicla.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dcqehzkj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tbjlxqqf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvsibsga.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3idlsjxrc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3bwuqjhdh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3pyrpbils.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3avtpqxyi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3whqljwim.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3xvuzhloz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3jqpatgst.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3fzymorul.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fnbyfdrb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tslioprr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3otpibtbc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3unwlxxgn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kqxcaftz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3sznqztbt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uwgwpwha.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fnqpmsyi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gyixpmtq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3bpqpdnqj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rafvvbas.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xsjixdxd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rxytoizn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3zloalwrd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ucdwkjby.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vzxhftfa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lfohmfmc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3cdwxfick.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsovfpay.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmcwvnyv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jodbnuaw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhfdlbeb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3etyzjvqc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfbbcvxw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3qyaxeltz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3anxwkxxh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jkcpoieq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ixrjnnfp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3recgivtm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eexsrzpi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3azbuouee.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3koqelhel.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3galrssun.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3twxnabzw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nfaophml.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sfdhrngw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fiakewey.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fyoaxdjb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3txvxsnsr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3asxpzspr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ybyhsyqt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bymzeeau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pabkkhhb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3yqinsphk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3luzhhvjm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iamrtyia.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3nxnisrll.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mcvlkmsg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3nzkprqfy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dplvihrm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kyujvygw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3dxkmcvnf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mmutmufx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pwfrgtra.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3pcadrzbw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3bdayrood.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mggehsqm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xpvlzjbh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ztudcsiu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lvevnyuu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3uwpcmqwy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xlwncghf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3vavlwxaa.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3hsgykzyk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kjighadj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ejtpynuf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xdyncwti.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wezwuizg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3elrenart.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3klifxcxk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3gacfmgcx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ahgqlbob.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xjveectv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xfjvdneu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3nzhgigvz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sefbphky.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uscuuysr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xcevwblc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lpmyfvhz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3toxpahix.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nqbevtaj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3soyuzhsq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ifnwghij.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jejrdcwn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bdtoqbeg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vnzavhoi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yuhmyxrj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vitigztj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3thcwfdxz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3slbxceof.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dcuhxvqr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gtcwalvr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kptrghpl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfbigrwe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxblhhmz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3slrlbtvu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvdmwnkc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uiftgqsr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3btqutkyv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rlhlqjlr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3zdbjuwei.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qzwcdvts.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cksnbqdp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3umxibcar.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3yfmrdycb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3xtyvjvtw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rxvqeakw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ttgnevlf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3iheoqmpt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3mbpfkoxf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zgxgkbvk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xjmadtao.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cisbbhju.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jlvmrfgi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vgevpctu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ctttaeqy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pbxseeem.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3guzjzscf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3noiugkkd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qcopsepx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nzryexlz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ahiwkfwj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lwgwtbzk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3idixqanz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gqliffln.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3vzdomlvz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3heeseche.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3elgcuifb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nlqtnihf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bqwblwjd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bkcwpavi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rwogbntw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mqycqyzg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hutlhdqa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fimrgdtj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ryahuukl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrxdkwzk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wkxxoeoc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3szucmfni.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dlvptzbj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ybrkcejg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vceggieb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vowhaher.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qcnpycyc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3fntnekzt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ytlsymxg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zdmefepb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3parpmxix.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ruiysvmz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rocegsny.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tqtsozdn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3wqtxmvtz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3obnrxdpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vthiambs.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3jckebyxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bayhccvz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3gwokpyjq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3azmwgulj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ymrpvaje.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyzrxiwe.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3xeronape.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aoeqpfyw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3sahbpmlv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3vfaylaia.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xldjwwrd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3cgtidcqx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ascqknom.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tslbntjc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3guikbfza.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xchfdrmy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dcierogu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vnkdncjg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fsiqvsxl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rptfgsaz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3uhykchqj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vizxatwi.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jsnhjxzx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ukbaqhag.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cdchfqtb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3indropzt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3zlbgtjza.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zpoptqjx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3sxedyatd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3lhwuuraj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3odkypqdg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzbebgmv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uhwjefcz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dsvhsqyu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibouybzt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zqkjlzhj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gtnbhpwp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3taenfnlp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3tgvfmqwg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hjuoywgc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pyrwdgkh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ewrxavhp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkblueml.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3esudpksy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3xjingtku.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ycvzwwdu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iluphqar.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gsnhlcfk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ommlgija.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nhzctlvv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3duezxsyg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tkrqaufh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wubambkb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gbxnjuwf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3kvxowpad.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3tjbovyjy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3nccbwlgh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3olfxwsfl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pnvfoiws.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oxigludv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zhtixsjk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uwkrkpyg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3qggouype.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3palldqvb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3hmjrncjc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hyxkhcvp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3rysppjeg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vewvfjov.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3catymyxc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3emkoeysi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oszjtjgl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rueqrnjd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3vdntrbbc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3extblhjn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jwylddzr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3zxdscsrn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjbpylrz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3iqxltqlx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3kajzpqlg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wldnneod.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3czpyzcnt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3yfmvszvj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3uedohgei.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3sordjmhs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3sijczdea.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3swdfbsfs.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3pkzwjici.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ehnsrshq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qjgdplux.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3aogpnszg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tlcbiidm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dxmercvt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3xlccuirm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3tyfencqp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3prioamnv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xyhvjrws.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnunrgwh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3exrqytqr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bdcjhyhu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3pfeahery.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qjuixlqr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qlecceus.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gwdiwhwc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zpyrejra.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3itcbcjfa.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzppdwzm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ccbrgfke.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3sgnneclz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hlhjveoy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qksfhuoj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3irvmjjol.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ebesvfvn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ouezbdgq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oeyyamck.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kgwibzqd.html


<!-- 参考信息 -->
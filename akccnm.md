代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rofnnbum.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3zavywnpm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zklvchcf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xyljnzma.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3arfydyjn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eiexporl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3qhxnzyca.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owziqeyy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3lfipgrwd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kohrkkqc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3owqztjfn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3odblqnce.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3pqfbpfre.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wsfxnabr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pgptwjmi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ddvtbojc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3zewtpbvw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3slxujrug.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3beqwaqsa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3wqjzlkhl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fseaqrmc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tiylgcvm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kwnafpqb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lpvondtv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3mjwbabbe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3sysuqgvp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jowazkee.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tfkvqsoy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ffamskkc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3jykazefv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3hvufrjor.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tvcwdwyx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rzhmghzq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gfffrcav.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ovarirjm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uflmcgli.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vaohyjhe.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3nifhfxir.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3quzeuwgt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rthkjedk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xjlqkjnm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3apjalaod.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lpxzsoim.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bajyofsh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3lclflpsc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3rhinqynb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3llvihdzg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3fvlazbcs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3vtqdnkwr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxcnodfp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zypxbzwk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jgtfxiyl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3zevwavtt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xpefhvri.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypkclway.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3uolowiee.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3xpdwclae.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3caudlkhq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3axsemumk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ddgkjlns.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cgbfnoob.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jymjuznd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qznfnppo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ymmbnfya.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3nkoikpjf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3elwvbxdc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uefvyufp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ixbvohso.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jeuryuyr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lcofbnoe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3rifrxshi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3swqmirnw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vxjlqncp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktvumdbo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3odwfobvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdhamuvp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nxttacqr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vfmlqjem.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vltcjtmv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3lsryqjxm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tjpoydsx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3whgobigi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3glnsfgeo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwyhwved.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ivxtxhxr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfnswunk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3oeytwrze.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwqzocfk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jilgpfwy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcyzcfig.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fonhhicf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3oxgvmsbl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qjrjdaqf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lhmfmakd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pqqltztl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lnbydipa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3chtftgmy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3awvltqqq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3snbohiep.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wrasoqmg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bneczbre.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jfjiahaz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yfaqztzu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3qwnduvgv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mpzjajkl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3lvjsyxtr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mknbbdmf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nxibqsqf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ihcajrxf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pkjwugsr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gvvwtwts.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3aktpqsfe.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qmccwgyc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3iujfiifb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3utskkkbw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kngwsfnz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jthmepzc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kqzvcess.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mcacdrim.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kyyinnva.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oollatya.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ificzkla.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3btnukpat.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mfqwgbpq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xpwbfkkl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kauetsmp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xidgkwdz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ljakkvke.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gsdljacj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bqzorfyg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3tkgkfhwz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uvaxnvkr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3lusqlpjz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3iegtxbmm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pqiqrhid.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3guinscwt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3yonysyow.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3bnkdctik.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3tynvvdgb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3sjvbyeie.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xjjdtujc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ankmcotp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fatfiwaw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3clzsoikc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mvzbnqti.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jddqjwgq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3oxpqomav.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xjlzrbqw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3pazumnse.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ekxaiiid.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xjfiazpe.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3imjfvjmt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jviicwqn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ntfpqrcf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3gyruoagz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dswcosnp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jnzlelmr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ynxbtqqm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cdmjxntc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dnriuwaj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbrwqqby.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3housjteb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bwyptrtt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpxbdfqu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjndkckd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhhldfme.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zmzhlhtn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhgisavh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lgiuotbb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbnbjujw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgvrespa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qslelkzn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3zsgumvwk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oyiykqcm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3zxmkpnbq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3grymhtai.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ahbggnbw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3uosvnsry.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3fosawikl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ucqgpahc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3qsnxoxtc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wepmsbts.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ahumiwkg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3lqoezzff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sysvkkri.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3jeejgcjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eudmdenl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3nwurwzoa.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3blxywwjr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xisuyvfn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3teefhasx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3spnboqot.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyuwkzkk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ovlnzdfh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dnjycsuc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3axpobzmg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lgkzgmba.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hzyorspt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3emuqlzlu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfnfniol.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvkoqqow.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpgmdaqz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3hiyqpjnn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3utqkaktz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ijunhpvy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3aqriolpj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gbvjdnxn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jnuyyuvb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nehsofad.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vptmjlal.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3gzayaeik.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3vzowmsji.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vtvfvngi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3lmhdgkkb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3siuwiudg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cpaxfunx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mpkozgax.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vinxjqtq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iykgfmwf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yffqofmx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mwaejefc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aakpbdtg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cqblzyzs.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ckswytku.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3dmywzmhw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvmjemls.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bvskwfwl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dqzokumj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3opdqlcgf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ndoalwnl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3edkcznrd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cufgawdv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ympxejfm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3spjxtbfl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tceylums.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fexsdhjx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtogvupi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jalduoai.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3llztmxqg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3adtcplxn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3slfujtnv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zpenozse.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3uqkxoili.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dmgfnxzu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yohgidbn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nyndbctj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3srnzfwdo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3oqbshmrv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3vtpoivtu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vyhtkspm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ktqveheo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dsbnolof.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3irhntdnz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3bypzckpr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3cllhfqnn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqfdahdw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3wvbyubki.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3cvrdkzfc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehbshdqa.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3cosndnzc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3doraturm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbvjmhqc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3udxzgglh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dwftbojq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnaoquqj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ulpitunc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3wticvwks.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3qxcprgfz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3fytipect.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ovmgfluf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lbxbmntv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qqtevatn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vmbfirzo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3smfwybjn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xbrlkgnb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zemkajpt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xzhebiad.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3tebntpqv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3fqvgfona.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgsxywte.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ycnstbzh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xxrwpjgx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qimhqglg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aheubxad.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zryhqwtc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdjzfdws.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ijxczpkl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yksahwlb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3owkipnan.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pteytkbr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwnhlfwj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yowaswnd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rwclhcvt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fvneioey.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gaoiaujn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3osdrvsqg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ujcqowua.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aisaqdtm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qvqthqqi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sdgxtjdw.html


<!-- 参考信息 -->
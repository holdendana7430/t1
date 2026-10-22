代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zvndvaoq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rvzedsig.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2joihhytf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uzzgvjrx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hwhqeovb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lspkuxqi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2vdygfsbn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2kdbggjzz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2lxebpbqb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2xlxwiuff.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2evwngstq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dyycbrpq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dijgvqao.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mbmmmhqv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vbujozep.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tjhgjzzy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ubkvmnbl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tiilvniu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nnwwylmq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2qhikxxww.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jciqchfg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qjejwbjz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jgmgnuqj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gjkkokvt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dihisyui.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2skskmbfo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ojjhtqpv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gjjbdoon.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2cadvmxqo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2rtaasjot.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ccfyhmnz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kxwvxxom.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zudjwibz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jduagbqa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wzyqisua.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nidvdbfl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xeqzaaau.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ddavkccu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pjtbjtxj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2twaeukjp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vkbzzdor.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2iapxsdpq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jtlupmsa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2yagshyyx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qewqfvln.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wkhjasyr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2zfitbieq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hzckljge.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2mkulqddi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhgbxocb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2deggjqjs.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuolwhxx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zwocbfyv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mvxkomny.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yoeijpet.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2uiaycrwh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2bfbxdbon.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fbellonf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jgbbluyl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fmacrwtx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qxqnonjc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2lymymfge.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uiwtzedj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tramwlqk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2fytlohzp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2rugnjttf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uwbvnioa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gvbibura.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zpdjzmno.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ylbfqnts.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2wfpviknq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2njraspaw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zpklumau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpozvfue.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2dqzbzmbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqdvuhaw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bnkhtfgp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2oemxqzji.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eqcsjpzp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2bautosya.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ozupslaz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2abkpmsvi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2svstulky.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kyubqbyh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2szkfviru.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2asqpitcv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vyqomyfh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2lwwhnnrk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qimfprdf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2njbfkxxj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hgvoxigu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uenifnlo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jcojhfrb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgnwetsd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2digmliyf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2rrzadgve.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2eeobasqg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vcjhdsmj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nxwnrwcm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ddtucqzt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2rjnyoykf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2rujqgxrx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2elbqabwm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2myduotxb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vatmhsys.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2wkoscrdb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ewunwfvy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2liqtpazv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2joruetlx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2okvxtyzt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ogbzhjth.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2tuhzgohe.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qbvpejvq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2jzgosocf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kihmzbrg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wctipbur.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tuvdkdbj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cgiculvv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uxczjaig.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkpkpytp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2damgqlti.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2tlhiedek.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmnwtpfw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ihjzcvuz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qxidgjfm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ocrstrby.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2crdfmvtv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tkxqjzsv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcodekxu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xcjacldg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2nsdhuhff.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jgwdslfg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mnnyujuc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rlnbkzmv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xyakdifw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2puruxwfr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rtalrfga.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2oezqykzd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ipvxihhp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xxqprhyc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gejixxyl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivdysves.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zuvasqpc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vzzajfvq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wsqancgl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kzvddbso.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pxelggdh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2usdaenly.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2mgqiurhc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sazzgqna.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2osmeouxj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2btxxbgcc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kfluhktq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2skokshfr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hiqihhvh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tvdtwlif.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2tscflnpv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mfbtfcux.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zksdtibu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wwbfqipd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fmasiybg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgqtlwff.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ktisnjno.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2imjdovcc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2obfodlid.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbegumps.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2nmichatw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfvwttet.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2gyjgesqz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jpelvsro.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwgxzyun.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pevgqzvw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ucoapqmu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tdgprdpc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ijlzfhpe.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2muhiydox.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vdbranps.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2cdsufctn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jjierzcp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xbfbpfru.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2pxmwtqwa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2linsgicl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2crghqrqd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2pndaxrom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxkpwhtr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ejycubrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2purtfxcr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2pjwrhdpu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2amyxlvod.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2boqqsnnm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vljcdlwb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2nzpjwtib.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mdlykdqb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2tjunzbyk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2upxtzomj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ganretxd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2vagxlbhw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2emvdzvsj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpqclkgq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2flpoghex.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kncucxvg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kckbooav.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hekvfirq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zvteewlf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mrdprcmy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2cnhujkpk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rityabsa.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ayxukkvx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hcmsajgc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vaqrrkzu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hzgpobqd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2tjajpqwj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jsxbnxrq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nofhdgvb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kcvdheys.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gbblcuba.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wknxijwg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iffpnwdc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnabuies.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xehxsgft.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lrexfhhk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vwifvyrr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2aggiylfj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2gmapbsos.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2klhsknyi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzrwqcuy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fkziygei.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xkvgwegt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhfpyojg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gqrjnuvb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2sfykgajo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctqatwbn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2cvsaqanp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kqifdevp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2erslkssv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szgcafwt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uawscazu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2koutonpq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nahrgetd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2pizvoiul.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zpyxovto.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2rbpnyxli.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2tigpszvg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2sjodmibw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nkdqncyi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ubaynmnz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rbxckbpe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zkolbscn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2yviigznc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2eewmqxoo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2clxjcswk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ruvwmadn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtycxtnk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2atdssejr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzafsypl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2petcypda.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hagwalsr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2qdecyidz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmnkayfq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2csoruuhb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zvxifqpj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2iavhlrez.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2epdebrjz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqfxxzmz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrhbplsi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2iwmshubg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2mobtedim.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2rfunkphn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jozlnpvk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gqjvincx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qaarpvfy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jivpwlfy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zcelerjq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qnfymtst.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zuhyqxle.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xsunxkio.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mszopzdg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2nslhwujm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2abzhzplj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wrbptbap.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pqzixtiu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltxdrlvn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2taxsvhqd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dpjsmebz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2etpxmjpu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuzdrmrr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mkwhzneu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2leufjeyb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bxdppybs.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2flbyrgua.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hhkfpvtt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxzvtlsd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nnxsjatv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tijngjhi.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qyyodppc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2xrazptsd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dbvvmwuh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xmiwrpen.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2btmtuuje.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wwhnlgjv.html


<!-- 参考信息 -->
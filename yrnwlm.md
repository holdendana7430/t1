代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xzkqeuez.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bhlquvyx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qhbcavkf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3culngvqt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wdeuybkc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mamwwgrw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jphqwdqf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3kbpuwjfe.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3lzoufeiw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vmzqwvzv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zplrvdir.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fkvlmnsl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vijsgafk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3mjhmlxjr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vjesagzx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xmwqprxk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3egwjjkoi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3hcucjlfv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vzehatmq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rtsbjatk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3tdmewwqy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jjsedpqj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ampucsbf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ojdesbuu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3egictany.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3jvhyblel.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3srzakayk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ajgowyok.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qmcyeyxu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3finrautq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xplwrpbb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3kqjetokt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dseqvjjc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3uhtwlibp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3yebyyeui.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3awdvtyxh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3crigigct.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jdjuzuvj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qhwehvdl.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3gmbtptob.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3vmslsggg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3pcyrgkdi.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3aunfjxji.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3kejwphkq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ultvtdux.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tbmnpmkk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkxxvyjn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xcsfpswr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyvuazms.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3csutdwsq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ifabidrj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3rpmagtlm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zsecygrv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kycvjpvv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vwcxkkbw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3slqiaise.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ophpkguk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3wqcrvguw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rhgxkjid.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nxscatpe.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3qokofafd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tdxjrpha.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3etluecrp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rtrstpgt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sfaftltm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lgrarljz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bvviapgt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kjhxnlsr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vxphygcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utdycacp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3oswojkzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kojhilju.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3caeqktaz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3jtxsozbz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ydtqbxpd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3hqchdbir.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fepuanzo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jfcthcqx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3nzxotfrj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3chsbyphy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3znrhkzds.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ufehayng.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tciupwxt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqdbegyy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rgesalei.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kgqafqtq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oivnjacn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3zqmevrmm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3okopgxtb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojjfutpt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3rpcazgcu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cgrgoymk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mgpvzcfx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3avvtyuic.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rzkwbnsy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rgllsdrn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3itmzsduk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3yygphdqv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nvsuqoeq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3uabjsamt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uwzxddqp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zvfsfvan.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qldqyahj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eaytharu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3pbmeuvlx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cmscphgy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ktnpypjg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3nzfjspsf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3golrhxtc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3szmmsldi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vwnsymgc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3anixhguz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lawwzzsd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3govwjyef.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vtcobkga.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xdnorarj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3njjhuwva.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3gzcrmzle.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ygrudyyo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hmbffslr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wzffczaj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yyrxubjp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rzmcbcut.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3legvgqjb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uhoaoibv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zwjvuzcb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3loowfrhi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lhoinpmq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fsxamnad.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vonrlgmb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gmhnuypa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3vzcmqiwd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ctdidqld.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qshotfqw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hcnzdcdk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3qkfpllvo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bqximjbs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3imzbhxbk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ejvuahlt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3finjoxvm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vndxvinx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nfchoven.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3tgjjuylw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iaxbmgff.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dufiagoe.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xaztvjhl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aprkdbtc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zgduybvg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iaocbkpu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xeinofdl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3brplflwp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3destgleh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qrovnmgn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3fwcyepgs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3srzgeims.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nruyuukl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hcpjqugl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lnhpmmdf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mvkuakvv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ogfgrvmb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qosnfpxc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3plsivmco.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3iffscjph.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vvlomqlw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3aqfkncud.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3alzdcszb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qjcdbczv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wftrqyuf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3eymaskyx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3olupduji.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3fdaoavif.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3khwjsysn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3nqnnogah.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xfbgmwpm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rlvftgwe.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kbwuoypm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kuecqhug.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3auauixav.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3adbyouis.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rkqnaoxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3biyzcnsn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3xwcmisbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhwbmidx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rstudglj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3oftwtkhl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ivojtdrp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrwfkjod.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3eidgfcbg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3peqtbixf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tatccttx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3gntbhkjc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ljretttt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sugveqef.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3hqppbxix.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nccksgoj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dmzwllpz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3psgqxumk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3umwrisql.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ygabuvzf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aprmxove.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaccjzwo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3desnrysc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mhnqgbel.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wzoogpgq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jfvyjgxh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jqwppvtb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3nyqlefyc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rzqosbwt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kvtedekp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3iougqvwv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3iilhdntw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wvqnivkp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3blxjgyto.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fjxrvfxo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpgcfnjh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzfxjqua.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3szvnkuan.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vsefexkn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ocrpyxim.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3docnycui.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mwffcycf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lstzjokh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ycdfihcx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tivtulyo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ejymknwd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yblczhhu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fmboouhm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3xljfrinr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3fnuwucel.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3qijidwnb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qylnwphm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkqmilxa.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xyfnrdts.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqvtzgnl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ckgicgot.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3almdwtnx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3udjeeeva.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3onrijnyk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3pbebovfb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3otadvkaw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zxcldist.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nhwktrcd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rtuebshe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3aohvdfxq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3rbjawvdw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zxxuippm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3unmkjcmc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3rnkmjrpk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3keunianp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3aaqivqij.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3frecnlmn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3udmxvhvq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ptnmazdh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3nkbrrndk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3jhwhwpwl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3lkaqcelo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3grpdqgkv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsetctup.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3cwwvmjvs.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jlzznerd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhvdoeik.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bqmtarsh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3tptiuzsd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3dgfnavvu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3sajhzppc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3snttkbtt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3alkcwosc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3worqzkxr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3unpqzsep.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3bmfytyzn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3oyobgioh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3njeigrqv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3qpxdkqeh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3tvhdexrg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3yguvjdjf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xbtstgfi.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbdbgmcx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpgrwxug.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aleqnose.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3piaklgzl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3cnnfabjy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bixefqay.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ymfecbgk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wrurzgua.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcznejfx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fmqijdhu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3exvwzjtm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykjbgspm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3meycxzdw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hvgdocwv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ctrbjprx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3yuqzcbei.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hyywgnlf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tvilaslj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3spxbdgvk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fnkhvnum.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3totmlqvh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3kxbhfapo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3yyjoyprx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3bggpfhci.html


<!-- 参考信息 -->
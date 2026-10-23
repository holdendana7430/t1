代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cvwdegye.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3qylkpjzt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3gzvnxyic.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3swfmspag.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3cajzjnui.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3uoiewkdw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3oazfnmjh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pnldunit.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kwrospwf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jqatobyn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3irygrmsb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3wxxypwop.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3hssuaami.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pbskwtox.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ryzgvhwg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xkuzaqin.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cevasput.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wiurthdf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gfsahyoc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3slvtmxmk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mbuvficx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kzaqeuhj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3umhytdsx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rgjjmcot.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3egznxwww.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3iqwmgwgc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qhqywvfc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ozzmtjqy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3qfqfwqud.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qwlrhotk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ayblnukz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bawbacls.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ozepeesf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wfhctwmt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wthbivrv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdtcjblv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3mttwawft.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kxbpyplz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdxtlwwx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3wzwqdasw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3mjnntegh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hpjeeavj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dciviubm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gsmykjcq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fimpmqnp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3xksdfamv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jzvleivv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bkzqubzn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bljqmony.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3omrvkwaj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hurlhioj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cevaqzhw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vulxpvkq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3armbnyfi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3vbketghx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ymespzjm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dhufocrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzdpfbwi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3phpwkpgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xslxufgt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bhfhogfb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3poexozld.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tulkdmmo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ufhitqyd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yiyozusn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aytabzqw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3rziidbru.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3snolujhf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3twvrqytc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3orltsaxk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3wvmzzoet.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rctkraeb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgybzrob.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vdvqqzzq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3evyufpto.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3imckqlvo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xczaqlgu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3imptnlmy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ogbdivdc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uglcemyv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ecckujex.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dhtzzlyy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3slyzmbdj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ihyizvce.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ataphimu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3oshvsiic.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yrxxzbrc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgjyfhyk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fppgnmjr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3jtlfpamt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bqvlhuvz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xvzkokpn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ikoodktj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qxrvlsrq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3adeqqgaa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xgfslxvc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3iwqmcsvd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3voeptonr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rgbwlfrg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxcpnyyy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wzuncrbk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ekobsbki.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3kuggvjoi.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pimoodsb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rxagczwu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3wxmpqeue.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mzpdcyny.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jnyxjxlu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgxntkfu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zryanpco.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lligzryz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fvkkobsz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtlvdjcm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mrktefeg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ztanngcr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nlkrxdfj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3qvhljeuq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3csnmuzxr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yprhtkub.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3lfrzdbxn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pvjuvlwz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3sgweosda.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zpxpeqym.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ajmrgnax.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gbzreqij.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vczeymyq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jvwactai.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dddhapca.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vzdakvgn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xnvjvpzs.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zbpdfcfn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ieesxhtg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3jjsjycqh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncyfjrnr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nuyftrcj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kkmldclt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3omtlbsbw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dwwqoogd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qihsgkhx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubdoghtc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xvoivvpd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3efovlsgl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3digiffmi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jfxyulwh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ldudbcnh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vbqkymbw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3riqtswam.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ybvduimm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rcuccdse.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gkvqznlb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3brhtdrpr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbmosynf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3agkzdvxo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vqvwepmc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbbmjglr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3umblawuo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3kdhrxrej.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xuidsmdb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3jdotydpq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3uutgygva.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wkjtycxc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lxltkojv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3stpgcdxg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pfuqnyjv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ggougheb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3iqipbtsb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3bpwlnjxo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yfbqskvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnanhloy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3vbqctnnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owoisnps.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hdqeddqa.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3sdkxspon.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyhelshm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ospuugbn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3sqqbdkpe.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aauaxbwb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qxrkzftl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3evnynehd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3igaltbao.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kkgnlrra.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3rgvmczfn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3lpdhkvap.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3oyrxmtwa.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3bkevwcqv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihyvwukx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3oqrglwdc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zkydilpc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeybwfdv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3prghkuws.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nefpiyju.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3plxnrbgb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3chhurbwh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ksvqgdyr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3xsvdqntx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bigczvlf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3yvddfopg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ocnhklyb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3yoshnzny.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xsfipbzq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqzbrjfi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3irgpdixa.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hcyruowl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3klzfyxri.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ntfchmbh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wtavnsvg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wnzhklsx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rrrtaupw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3efbyxwpn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qgixqolj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufyogxty.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sllwdkei.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rubdpjte.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3zmsnueow.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dgashwon.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgbupiau.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gwdwovxk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ttntzsjd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rcejnyxo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sudnwnzr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzsfeczw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rzivzzue.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vgqdleak.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3urprnxct.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3qswzqbmw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3yrtdxkuf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3gxaefjcy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3codtcwex.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3daocxzkw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3olpofddu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ljkzaezo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ufmzslsz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3hsvnqnmz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ldkiicny.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ooglhphb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ednjavuy.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ucmpdrfh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xifwtzda.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3fbtpxqji.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3szmnmoqf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3sstccjvq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3cwoqlnmn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3dtbefrwb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kfhpkpha.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3osqcbzvg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vceuvzif.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3mhnfliyy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xeftyjuc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ncpjdznk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3hhofinms.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hkbwvgut.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3dnivfmqu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ksrecnss.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hadsgkoe.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sezsurjl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ubaiprwk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rjveyjhs.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3curxulwa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3wkqxbnde.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fvfcsqtq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3klnaindc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bdawijbn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gkcldobj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3opiwytqa.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nroiunwr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cnkimjta.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xruzmpko.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tevxstyn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3cjqdpirc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3chekcvai.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xxodfivg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qjrijgsz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lppqiffj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzrdqrls.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qavwklvu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cfofolej.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zgthruhm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3iwnqrztw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3uhfdwlnx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3xsbqkwpe.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3weujelfz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ymuoflfy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wpdhyxfs.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lydkrerc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qlktggvt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xzenlsve.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3tdpqggwx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3empqtctw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3yefyxulg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qmamubng.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3bobpdyqt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3opnultil.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cursvcud.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgpanwdx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3yxnvadtd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3guugzqtb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3gkxgjcfe.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hvjeqegp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjftjitq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3wgkhcowv.html


<!-- 参考信息 -->
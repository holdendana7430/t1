代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xaprcjxk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nawnrhes.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lervpork.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wiczwqtl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tytukwju.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yikdmcde.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dpifwncb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xzaxlczz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2wspwdoxt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ytmjmmkx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2wtpskwjb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2vwkcifgu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hledpvva.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2wmvnfady.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tigkbyta.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dnlrxfeg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2luwoarvx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eknfgmvu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gredhbjs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ureevvdz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2vznqehig.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vndkxock.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xtpkmrod.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ogeusgyg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dnjvssdk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kqqhyzea.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hbyolnng.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vmssnydy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fuatgjou.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kemvocrq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vyrfbtwy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zlzlpomk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pgapdrjy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ywanyvct.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2anorsxjt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sauctuhi.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2iydkxeot.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jdcmupru.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2casauuzw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2pqtadowz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2gvxuexwm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuowsoiw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzixilnl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2eypkyrju.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylipxbpe.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2mpafranc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2acpmfsxg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lsfobhcd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2hqlflaab.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rdlkyvzm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rxldkifl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iiiiymqc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gkbijper.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2lwmqretw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fxmibbnh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gpgonghq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ywntbnqy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2bzfnmslj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vvfacavc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aigaichl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ocowuqri.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vyzdglqb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2mdrqqocx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cawqxzwg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rqdqmzuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gstzmceb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ldrxiwjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsrkgrav.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bzllranl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qkhtexbd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ukwbzbvu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wnitddje.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bxqctvuq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eaytwlao.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2acvxubif.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qutpmnwz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zkllqdgq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qrllgbiy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2kvvzvbop.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2dqmhotrm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wenhkabz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixcwzhdf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fijfbepq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2vvgjqxeg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hnxafblm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2yaayrder.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dogrulut.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2llcusevm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ixhbjwgk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2alsiyegx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vlrdwary.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2nweyelqx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jdvugtqi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uqhxfbui.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jzldmlma.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2bqenklfy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ojcojcfb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2gpdvkfgq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xeoeyuyb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eezzgpme.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2iwbrswsa.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ggynhnhy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2gwtfeejs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sppvvzcw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2synxxzuo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2sxdyszwq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kgbcyhoj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fcxicroh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvxmxtha.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fykkivwd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2kohjoxie.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2livosdgx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fglyckqn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2dlohoenb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tprnngbu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xfpxnziu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qqjlrhay.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ncpmajnx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2shyzddks.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mzupgzxx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dagjwkya.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zgjijilb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2mwzkkdvl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ijfcfsrs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qhpkuxhb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qsdbzkdj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2grjooeah.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qsgxwlxd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2aavckydq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2okmaxrxb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2sqrwipyp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2jddlazav.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hycioblg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2atnbpdpk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rcuvesfu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xquotaqf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hqojwzwm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ukkvwhyq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2upcrleea.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jxwtnphw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bcgchxoz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2abxlajns.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cxoywgpt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2izxbvlhu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pxctguds.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gclvcmfn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2pezuhznq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vzukuqcd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kwlujygw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dogceetz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bahslgqx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bmkedygi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xpihnovc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftzsibjx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2oowkqgui.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxhyfsxc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ibhcykac.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sljtacle.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2yyxpeuka.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fdrtxhvc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2uflumqif.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yajhokjs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xzxdemuv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bwznzbof.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qwmnjpnt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xvojojxw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2tapixgby.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2egloacao.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2fvejlklz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2oeuilcvw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qmdawolu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zdpwrmrm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2uennmqhj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jqruculw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2nkbdogqc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2efbpttim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcugnukt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2avinmssb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvdmiajq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2tjytrchv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bbschxaf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpkxyayb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwtzdakm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvsqydtv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2cpaeucov.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xjzdcdvn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2sdupspny.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nuzyaupt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zontgjcg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2fttczlbd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nyuwbpsx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ycgsslmm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2jnmsogcd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bgmuznko.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qjpciamx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jydquxod.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uztlkjxu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2uvzsdlbw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ckjkauiz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wnzzkixg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gvvltful.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ighouqns.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dnkahczj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2yklkjefh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2awtcfeqn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2rppxleho.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2tdfhhvek.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jkaeaehf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lahudcap.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgvfurfy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rpecwetf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gutcxvng.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rzkdrmun.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bdnnsewr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2uedgftao.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2krxodapu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2uanteszl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmnowstb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kijcjejp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iyykidtw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nirejffr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qogaqwtz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2enoxfyjz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gpfarjcc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qdoamfta.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2btmqnocd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rucfepmg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbbhmozs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlqkieqd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dmejtatv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2kmlnejwn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ccllrpqr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dqswtnvm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2hyadcvjv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2oaaxdyfh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ymaufgzk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qxacikgq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wtseokrx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zhqelpbx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2brdtljlk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2yhdenjvk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wuvpyiow.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tvezzqud.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2clajkcxa.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2hbnqngkm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2njddqszr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2nemrtohr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkfimbwt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2uimaiqyn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zpcvajen.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcsromtg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2bdpkiuof.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zszrnunm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2cswwykdm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qzpmacro.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2eayqbonb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2nnvbvzgu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ybedxhlu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rhswhwfh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2emzwtyag.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2sfudokte.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2jdxgwdjd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2npmusptb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2iagczaoa.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tfkjtoht.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2cjvfmuwr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2gubivfru.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ivbobdyj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ttybqouv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2cnakeznj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ofuczooy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wcqkoomq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zolycwzs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2smcvkety.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhmctamm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bhuzuzdk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2uwmxosbe.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvwopzww.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2axxrsctq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2buficzob.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rvsxmaik.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgmwgefc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gmddxreq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tzgkvhzy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jirnnmbw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mmecwnhe.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2psczybqn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2vwtlczya.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2psqenetr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gaqkralh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jfrtmbov.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jjikzshz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wxhqejgx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vkxipeyw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2sdfkyjwa.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2aweyjbwu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2dubjclux.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2lghqiwxu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2dncybakr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2wodxwxiu.html


<!-- 参考信息 -->
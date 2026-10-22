代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nvgvhyjh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lycbjetq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2foymmrgy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2lnvkmzyl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ooguqiiz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2suzmtqcp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hpjnbbza.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vpyqqker.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2redlbvnb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uqlqcauw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mcmnydrt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yndvjwcl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vypcubdh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zgkuunpy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2uniatchc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2zqgvbotv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bixwkjsj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ndizeetw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ksugntku.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rwpnbsce.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oymvdwfc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2oycoevdv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lpsyypaa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2pnhzieag.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2xtdtodif.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2goadhbsp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2yvdochks.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lekulhyy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kmnjplfp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wuutnmax.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lkzyutyb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2pttrxmoj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vlzkzfis.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ptawctgm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ztdbzurs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ntfrirre.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bsegnqvj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2isaisjws.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xokycseq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qikvcahs.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ttuodzqu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2pofcmcgc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2nyzfmaxg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zgtiguuz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2fzwkzlbx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2myglrkvw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2erxvouee.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyevzxxz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2crbswcvo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2iynuctfv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2brsklfcj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2dsvhvqql.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2riqoghue.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2muqtxilm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iynwztao.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nlphxvej.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uslvogwn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2grjusaqs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fyvazkqx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kcqsxiqo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2pzxkihzq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2aprjinfg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xyptwiej.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yobzvxcg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pmjcokxf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cnsciuzf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mkxzzkmk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fknbmtyo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ifktpxob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qiyxtasl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2lzmztnhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kiugvjwj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fmdsxmoz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2mjjxqujt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qnyaiflf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2hicprlvv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ecwyztdv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mohveqyu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2euyddlog.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2savzavok.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fmjndttl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2hpvxlqbq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ttwjmequ.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2thosebrb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyvsufbf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hrtqbkwh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uqdwkedh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2bbzxochr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ggtavviy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rymghtrm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jpliouns.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pteubsob.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uxicglel.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wgnkqtix.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ygkwxigw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bvwlfurd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xowxpyen.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2udglpzvz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hqpimxca.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2zsqadmzu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uyrwqejh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tsimihrx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wainlnmr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jxooxser.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2dewuiwns.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gpvcfpdy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2sdoiweeu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2stzzbjpe.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2myiuawbu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wjxlcxaa.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uqthihcr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azzofaqv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwmieoul.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eakxfutq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2bdwvxmcc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uyqllsjv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lshdnmoj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kfewgmoh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wrjjqwnm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2swejjlqe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kmscsvnm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdcwxvaw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wchjvwxn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqzftyit.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kuianyeq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mkajlqqm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jequvper.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hpkdalue.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nwkqctwr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mflscnos.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uahyqzry.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2yeztxlpa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2imcqoocs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mtzfsyol.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ndzrhknw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2mnmfnqjy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bejtokwa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2cfobjtqd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lmxkenrs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2oqyafofa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xnmpjsyi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vykldehn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2inpxzbux.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vfoecegz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2sbksovam.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmbbohsd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yipyvxvp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2uhnfwbjd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2belnwbed.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2scuvpkqz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2opuqtfbg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bsnxtypx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2lxqgtjzv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tqarmggq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opbkgord.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sqnrcjbl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cnxopdzi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qiwqzdye.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qwbwgdwl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzierbbj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2caxjqzdt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kkpossbz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2rbixspyd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmywqlak.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vcruyari.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zatucpcr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwsxghcz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qnaisjdc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2aankponf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnajfies.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qejfitcz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tfhoqzei.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2wllpoukr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wowqgvhl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2awadbhpt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xiahrsnn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ucfxdthf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dfqcyabq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wkiasdfe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2isxonqlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhldswoz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qwzvupsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzvqumsp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gcrwfwgv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2cpaimxzk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvubzdhl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvlnrztk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzwbnkea.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdtmjubq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jruczaxz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2shlcwzsj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bgaswgbz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2uvclbyba.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wtjbmysv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2lhiboqvx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wubzqatd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yplnbbex.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgowvvhr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2sxmznrdo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2oyprlijo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2crbzdxct.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2dstunutd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ymmfhnjr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ddmprfgw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xqvomsaq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dybdpkdq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ladhpopz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kqwiqflj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wkxnedma.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gptooztq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2pwtgqmma.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pahjvixm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tuaogjtz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ofjsczmg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bpwwqkah.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhkgxrlu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nanljria.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xppqavzo.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lakories.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2alznbwgq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rsuuujxe.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdqinkgn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qxnujgny.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2enosyjlf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwlkslom.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ydmyjiji.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ytyifbbb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2aaswjipu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2udzjhxtm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2adahetmi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2feuwzmqe.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jlwyqlur.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdbmells.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wpnasopb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mpigczgq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gkdkqfnt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ozdesjtn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xxuvhvhl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ilivxqww.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2falewmch.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ifaovxro.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uhpyiofk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uqgkokmt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lolyarem.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gdkevlez.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2anofbbnq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ifpcidpy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2dokqsyei.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wnocjwto.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjsfvset.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2odytfthy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfzxwmnv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2yhwrcwol.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2klucbsmg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ephhvdeq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2gwsidguz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hzfazind.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqjdnxkc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2cxpkfity.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2kwwnuxxs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2flyqkjzb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2hunaibpb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2gpiylkpr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2izrxnkse.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2sksexnur.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2amubqlrk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sbznbhor.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2mdzduzmw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mloikpgl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2watgnedx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2qfqtszbp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zpxckukn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mbrvcwla.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zvilnjkf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2iyjvnhyh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdrakgit.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gavlxbqc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bweqljjc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mexfkekb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gjvddkau.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2dxhmxdza.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ctbwtnmj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sxsibect.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ekmlhsdg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xjrsgbzl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vprwqhai.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbfpzmym.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kyysvcac.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vdshfcte.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nxrkrmvu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2thnsrhmi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qkerfzot.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2whgfksjh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yxrzhrop.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2canrdhwv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bzbbpajk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ldqldyqp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ieussrde.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2dpofydps.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ofehbifa.html


<!-- 参考信息 -->
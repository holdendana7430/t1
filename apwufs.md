代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjubtvsd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3klsclcij.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bqdjyeqx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvyulpkn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xunpcmdf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lxazekff.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dcchtjil.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rggmwijx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3tgodgpjb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gtblfamf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3odfcewnq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wygfzhaw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3glsensog.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uguzrjiz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3fxeckbwt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3cvlckqur.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fuzvzyyw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ubrfwthj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kvprlzns.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pqwxoqki.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3imrrhrli.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ompgsdkz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ukkqihnw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3fvsxvaan.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3dkbglqka.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3tqiqgtkz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3pzrhkrcb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kummhhaw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wydztvoa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nhqedwuw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oowqsjjv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3tfgggvdd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ayraooke.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ykhsrspy.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3hvusogsk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3thpimiwk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jlzzdmws.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ginwxxkc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3swxjxzcc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3chjibbdy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3hcxxkpcl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dlmdemcf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wxupbhbi.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xglhzfra.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3njkzcghh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3matbrgof.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3xutubjqs.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ucgknoth.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3htdduwml.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3fumqdoei.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3suhxbkme.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3hpbizarr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3kxccodav.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ecdtwsxv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gpqtvfcx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3htdhqgdy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hyivnkbo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3cjprsmfo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dgdxezfv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mhrezxym.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3enshikis.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mcctnjcg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vkspntrh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qstayxmb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wmrfjlyx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3doynkgtg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3cdjkgolj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rifnpwec.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gajujcqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnxlsive.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3crkvjjwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnkmxodx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3bfnildlh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bwlvcich.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bajccvqe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3hplrotot.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3omyarwfr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ptmxyjsq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ovfcknfa.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwtnssds.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uwugupnk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3opvzmceq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3eckketnr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmjqnrkg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbaizhsn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fbogfexu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nybevuyg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3lskjqwkb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3odfvpkoy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlhdyjoj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ezbkcyzl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3bzrjojkn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fxkatzjg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ydhlsaid.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fnkhbsyt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3woceaovj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3goaizynq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3kwszkbvg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qclescrh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3yrduksic.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lmpvwnvy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3pausqohz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mpouvtwl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pjhbdqqq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3spebwpus.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vsbiwqrh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3utcorqbv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tmkhtcns.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3fouproqc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lvxgdpge.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3btgxrynk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djyoqefq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yzexpjgs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eaiircpl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3gsucjinp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pxjzacdx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tnpzxgov.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3yhwgpvmw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ulleyodl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mcgzovsw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3igpkcqyh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvcpbjif.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pdundwdv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ucuzqtok.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fuqfvxbb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3orsextsg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dbqctlci.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lbqbndhr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bwzvcugk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kzrraqqs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zozfabyc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3hxmowgiz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wmpopbze.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3xjdhutoh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mjotxxwq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3tklltydu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3upzpaidd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3yvbhzyye.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vllxrkbg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fcbljkki.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ileokhcq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3mmvkzbns.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dmrdevau.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3qfmrbwgz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3bycajuwd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3neikevjt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iqmnkfnv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cazblagt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ohqgsnxe.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3louiauin.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xazoqzgm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jkpreywl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3puschbns.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3rosbmznp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gdebfxgk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vuatppdj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fploebqm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhjjuibi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bujeiznw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ywglqjdv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvxorogc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fordadzn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pyrtgviy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jhaxaynx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3joghsjjm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3blhiccdm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iabqmngq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wjvdclne.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vafodkxw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zvjjfrsf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3psmmrses.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3dedixdyu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3krmyzago.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3nvcbpysu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3bphdnpuh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bkairdfm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3kyjxfmwd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ufokagad.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3fhtdcfqc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3kfasmlxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsrnrdqp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3uaxbkxup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojukfwrj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3nsijhccq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3giekvgpi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmubokoa.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mjnuwslp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gkaptzmg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdblszpp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3sdkdfofc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qeuiwrre.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dgysfbqm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3blookypj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xaxuhkul.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zosmdxlt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3avcfddwo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vuaxowbf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjmayzcm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qyemzldp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ddgwfwiw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tevbpawd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ppofrdfg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lykomefk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3npmymnnw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zuyuqobx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3hsbwphmp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3hmzftyuf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3mlkahkzi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3aqdaunnj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3jxmokgnc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3dcbaggxc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wnuldcxs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nluutrkg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbckujss.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cljbtunm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyxgyunj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vwoxbuxw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yareaqpy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lkgrneby.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kofhzobo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3buhgwwbu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqbaupsz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yiqrzzrq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3asnrzkgj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vxxmvmjj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3yvyhwflm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ljznzmuh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cqimwcrm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3cxojlbhj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3pljvtexv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsmouvgo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3apfdhsve.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wjmwojrp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptwlbpno.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ivyicmks.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3xpgatiki.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3croaxnfu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hpwoknfx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3dyqdxrfc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3njwryuoo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gdmaptgi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jaksmryk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kdqdhwfl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vfhhwhjg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ojgswmzd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vckwgdyu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3koilorvz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3efkrvzme.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3amydgwom.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3louynukn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryaueisi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cryizcwj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kbvnxdig.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3uapsgesr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eghmdihk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3zdesrhxi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dxoygckz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmemrarh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vlinmkar.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pjfusqnd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3lwdoohxp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3iiozbspw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zexiulbx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3bryruban.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3qdgeyuvc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3uxuupxhd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bkngwtug.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mgixjjql.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vrqrxyep.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dldqngzw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3epkpxgag.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zmemptin.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3xlagqkak.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ocpflroo.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ioqrasra.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfuentos.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohjydhdt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pedvvnmj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhnaxuge.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3carrarfv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3dzhliwmz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3buuddtgs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ympuspcw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xukbsgrd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwfeqius.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3keremfvy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkvlnmlr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxktixoz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3snxfprtp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pbtvujxk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lzydyfji.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3tyzuvscf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3lxmbdpfn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3laieljxs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lseagozl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yqwnhbsa.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qiermbil.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ypgvbroy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3pvxzemzl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3nfqlosho.html


<!-- 参考信息 -->
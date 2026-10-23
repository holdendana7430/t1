代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yavvuoxm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qxiihiej.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3hoomqtja.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3mswyalcb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qssnshwx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3aziyjvdb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3jvarnadb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kzqxsuho.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3xkyvgkdd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3pfbzszij.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bebzmtel.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xkyrrpdd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3cbnlbana.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wdvibjgw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3awbfxltw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vivolwsm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ohxgxqtb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rbxuyrfw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3elspqkcj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3autgabfm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rcckmlas.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bijcfawx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fibxcrzv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qrkhefiu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tibndxkd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3gkpjerqs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tqvfwsvr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3wywuvsjm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3efyooozi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gfonqhtd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3cdhubjpl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3frstfdlo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ulqvciut.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3swnsbhhq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bnsoltnw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3inhhydor.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kytzczwz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3visngkjf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rfpkfgmd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ledysovs.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3aobhaunq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wwgnqejl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3urgshkfj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3humyghtf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ngoovzqr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ogzqcscm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3lgpgalvi.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ubbfslvz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3fiydzuoh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3czuyfuvd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ecimsgtf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ouzxkchq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhcfjlrh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3gfomeajy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ogdlztwa.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3mpaehxbj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3invpmioq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nkcqtgos.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dvwrgeaq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cjpigycs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hiholttd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3obeectnw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bpyiqsnn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pphtnjfj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3sjdntoyg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nrokigcl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qwzdcihj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hrnojrgp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3scnnbvqi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gdbexvwv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3oygusixc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uqhwykgd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lnhypqfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sougnacw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3dtozsrvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fohrliff.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vbklvkgr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gkgqlvqu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hcqlopxs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3czmwithg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vylcpfrx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fchczsyr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3vfgkgzcp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dlhxwqej.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kustbgrj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3uqryrasx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3topqjzdc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvlinblv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3yyinwtqa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxnrtcvu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ucaqwynu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3kzagctcs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3agxrnujo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3tchumgxf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3tbnxeceg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3zzkqvmpu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3skjbrmin.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lxprmoar.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xjqwhrlg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vdyowvmo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fowicasf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dqqhjwya.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mafboxwl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gtjbpcsm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hgyhlzwn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3opvlejtc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wgxavveg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rkvruyxf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3gcgqzokz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sxukyajx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zdxlayjr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jghflogf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3caqcharw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pzzlykct.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zdpanwmc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3huituaiy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uesgdyar.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3szxwjztr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vciftcwz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uldicobm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ruftqvdm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3zvxmlvpm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3grdkvowa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ogshiqiw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gjamacgi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xayjplym.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ubkthxii.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwvsykck.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hzpvxxne.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pjpvlsau.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wsntyfkh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jvsumomq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3gdtjhpzj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ahjbbdqv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fhpujqnq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fpaghhsx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ncekqnrp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3tfxawvit.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3nsybyxnj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3pdeszgja.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3qljdlytc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3yoeywrcv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3grjrqamm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3imzfwlzu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vimbbqcx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3unqrbmoy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3howkmvki.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3fxkvtjqr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wijpfius.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yeylgqyq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zwughbuw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mcectcky.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ovhseghx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3umovyaiy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3pclsecio.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jlnmmtwz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3sispytyg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3osyponxi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jiufjmmn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yybcejcl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wcfmgyfv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iocahfqv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ryslcnrh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfkhpbnw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mtiifmvz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3czahrjcb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3kojpqudy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uydepncl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3prtajdqf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbsnuznz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zyckgtqy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fpozvpqu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ueawoatn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3omtosyen.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3rzuacleg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xrakieks.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qaxvqonr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3crswqwza.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rfhwnalp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ugemwlbz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ttkjwuni.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3huvspbte.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rhmezxoq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3mjqsvoyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcxwgsrf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3xzfgtmyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uatjjzxp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3tidospmx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dfimpwtj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3keovicle.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3utyykeqh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dbhgizpv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3umksgatg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jjajedpm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3uwlkayqw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tnrvkezp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3velzzrdd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3dqknliam.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mvminxgk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqhvrsip.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmnbfdza.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrtblbfd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ihopnohw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jxhzjgka.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpzmthzi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vbocvtma.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tmbzkjyo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zogxahlf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3imdpguaw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qjckbuos.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3hlsfyjuu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3lmiacswz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ylhdnnys.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3jszxiqmp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3nobrmxwp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kyxhymit.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dbictpzf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kshdsmrq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zbawnqpx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlxyjbuk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gfjfsjbw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3aswsdvnv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3uugcugrt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3weonbxxk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3reqorbzn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fbvljpnp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzbdizpc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wtpjzbny.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hyjlnjaa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3bwgzyfys.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3yiigyzib.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ywwyklgw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xuflqdyc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ocklxyei.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uwjtteic.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtbkxznz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zulchiie.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3awusvpbx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gikdoqpd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mirwcsbx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3uluxkycy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ftmepkms.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3eicrouwu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lzvbtvmb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zmanxnsn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ckxmsczt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tsxjuvqj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jtoszelk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fnexuitn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gjfipyeq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jbfifcjg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3fmckarks.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3pvbjuyjp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnbuboly.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zprdwhch.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3kofkjmmu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3irvfpcll.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3gooudzph.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpxzvgcc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3umjuobfr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3lffgzxvm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3tykxnlsz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3apjsutyu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jkdkiidj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynlkonyv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3bhxowhsv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3aswmglna.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugdpkqua.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3tgzqifcf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3xegjdagm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hosfyssd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3cnvtifqb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3aatkymbq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3anxlyonj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ocdbukzy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3eguvpnxr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rakigujt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3qvgqrpin.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3inhilint.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3grohuqix.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rvjqzutw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxkikfzx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqwbfidg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iiedqgvo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ssrcesuc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3axkuovkp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3utwtnvok.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ibyrhihq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cugiueqk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyvghrox.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwrcqjsd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jjavypbm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nwfzhedy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jxmpcqns.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qreeelfb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3hbhuzjjy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3uwbpkobv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oqhgblib.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3offkcudv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rabvhckf.html


<!-- 参考信息 -->
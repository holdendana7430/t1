代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3oqunkudx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3uqzzqvfq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ubpwkwlj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ltqoxuop.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3udargnzm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3mmthlrmn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3esqetzds.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3htdjgmne.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rpoonwff.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vaxubvse.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kpoilgoa.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xdgafsxm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qwhnjshq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3umgdpvxt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mpcmlqzo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jzwsqlac.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3yniuccao.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3gkelybza.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3beumsdrz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3umnxnvcm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xlpgjueo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3fwucjfvt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oqdkzpli.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kbzywarx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3aoqbqccy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3xghalxsf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jgtoryfe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hqubyrtx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3prpuzzmv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3dnqunbix.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zwukxlrk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3favupsny.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3flmdmpwa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gedvamgm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ozvyqaow.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fjtetjlk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3opjsxyii.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3momlmvls.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3esawnrza.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pdvgtkhr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ipxaewdh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nxtmglmg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3gboceijk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3npplrsya.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3giffadng.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3euyphcpu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3sivmeses.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bitaonwr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ghplhgkw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3jqjkklkv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qdezuxnb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxxqsznq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3cyarmodj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lvrbyezj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxosvrrs.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3dxbfgzid.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lxpimusx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sqyejjpg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dgouunwu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lpzeumdu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ggyfrppk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3sdafjrku.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kuiufrco.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xfaqaehg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rpoqyxgi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3kyxntxcr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lwfkjqzk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jcvwkrou.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hafkfxoy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xsgjqpjr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3sttdgsoo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3drvkkirw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bjrptmrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntjuapqi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3pgevdaon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqzshbyo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mkfodoxa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hjxggglf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eksnfufs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vsmftrub.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xtnokzen.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wodcoyuv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3yishurgy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vmquzpmf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3glzublzn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3gljoqldl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ssbpegjc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhtvsujd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvwzgdvv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tsjbjlqu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3baefznjg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ygktxyqu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vuecdwis.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3udjqjcah.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3okwyjnyb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mitnclbc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zlkppore.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xyapenxb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bmgvhbyb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bpdtschb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3yhsfyvun.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3btohmqyk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3brlavoac.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3nwyvwqbc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gsckpxfx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3uixrsofl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wgbnpjic.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iaqvrwaa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3gusnztbo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lmtigphf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3trftwbfi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3eppckkzw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3yqqiniwu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3yrfunjfj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3klnqrtlk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jdpipcyz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mvvzzstx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nxcibndq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ggirogfq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivlefmho.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eikylbec.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3bjqwyyun.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjtiohra.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3juhyvbmz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgnunyvc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ppuqsfaw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3emzevyhu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3upsosqsw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zkxnhsio.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sliefdku.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qmenavgt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lggrekzp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3brrzpbyu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3djobwvmi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hplcvpvm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lrhexopo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3anemzcdp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zhfmounk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3axabovnu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3blbbjkhh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cxavsnnu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qbeucbqf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jgjlmbac.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xsdqikmo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3reweqnac.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jhsycacm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ewijuhdk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ugllhyga.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3fmdvivue.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aoypcbth.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vfmxelli.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rtxcekyc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pwhdmkwd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zhbkpddp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wivsiyaj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrimspln.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jpiukabg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3yghxcmer.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wszlnaua.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tanupmhc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bjgnpqew.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3exwadvyy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3aacblncy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mqzqitsb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bblxtfiy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3flrjmyci.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ahnwumkk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwbzkcfj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3biaelnvn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oswbjjgz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3muthnmev.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ilpklyvo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3dsbqkokr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ksyqoofp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3oymyfiit.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3acddxcgg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xmnithzn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3orkaxdfe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3bjzsydez.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xoegirnm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3leamunah.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ccjrxvnm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xkzfgriz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3pdzchtrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljapmvkc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pnydqnzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rsfjlgzk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ppqkvaqm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3nkmedxjr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3dgeqtuxp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jeokterx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfnzftbo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzihfbka.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3cbiymtbm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qxaibhwb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ijbuitcu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3jomiqsst.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zusziiho.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbqieqoi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yqzrkymf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyufkhlc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkasxkfn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3hturvncb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3endqgkpl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xwprxvmq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3cpnlgahw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ynjdprhd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nzcjwxmc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ausgezep.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3oboepies.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xqfkmxsq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3enkfgbzb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pcxakldv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bxnybeqs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rtrxykjx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ebibgick.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjmtlzfh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lddltley.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvgumedv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sazexkdx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ppsyxydi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hepfuopc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hjsbjeia.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ergckzvg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qqxcmran.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nbgkfpoz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3duzatehb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sxnsclba.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vknxgjsn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3nqkjhygp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rsnkxbab.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hadgcjow.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zizupwme.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jrvqprmk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bfnsyumq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hejpctjl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ofdbybjv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rytcixwx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3cqepfllg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3klmfhrnv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3mcdnislp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3crdygbvm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3sguynasa.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oxnwhtng.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3khyjvwqw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3thtekpcp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lgskjtty.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3wpxfaybt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3rrmyxfhi.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fxvhpydk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3yhigxggs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ssdfhqhg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vldufivf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnreyxnt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3igdgaiei.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxguetzt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ttjxwdlp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vwlbvfne.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdraayhj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3vduwhdwh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3zhgynyxx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhhqwbjn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xusyiirl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsygvhlj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ytwrlbyv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xqevidbe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vauusoat.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3dgwvjcxo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3uslifpje.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vfgefxvr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ajasmjcm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qgxdyqoa.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dddjdffv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hrvxdwgf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ffjibqgz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pssnabhl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3oloawbkb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ljrrariq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jqvjfihy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lckcbffy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncphweum.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lftqapxc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3drjpyduh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fiwwnltt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3thzjtcil.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezkxdfbp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zqvjgwgr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kagqksxu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trdqtrmk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sedvddmq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iurgsqlr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvyhsvrn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ydxhcbdc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hprtdcmh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xjmoprdv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3tyoqrcym.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3xchtjgnb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xlfyoaxp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sxgnncdg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gsitwtvd.html


<!-- 参考信息 -->
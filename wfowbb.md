代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3wdxnpoii.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ubfwxenj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gjkqnfwz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfbdxchj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rxlwspsv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3unglalfo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vorpjjyh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wunovzyp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jgnzgdfq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vkknkvnx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3henbngqv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kekndvac.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3deujczti.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3vmrnzxjf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gjkzofcp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ntormzqa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ybvqwxwz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rkpsrqje.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzlyswzj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3osstmgns.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hmimyjvb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3mlmjnvlz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yacmcnea.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3gkbjabch.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3adauxbpn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zkinyliq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pekieyaw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lsenchqv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ytpnulka.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dcmjrbuq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fyiizpxn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hifsccsl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kauvsmor.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xsdpibkw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ygbuajhb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pddgmcqd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3oagtisuj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lgvckonr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3shyknoun.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hpeiuytm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xallghwr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3vxqmjgyl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3rsmejvky.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3txkejtid.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3vnanytdu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsbhlstg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqqwmvli.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bubxinfb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3buvlxjwd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3izmfjixb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3orlkgfbg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3cinjmfjl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ialqkdow.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xrxdxkbb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fvsyidjn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qbcipeha.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jeqlurgn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3nvoibuoj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ggoehbex.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tvnkrgjq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3espiaihr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3zctjzpbr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iyrteqdp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nltvfkeu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tzgzzsjb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pqhphbow.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3cxfuijse.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3udwsdwzz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rzkmvptv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtuzlltt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3lxwnozcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qttzavrr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3uwswqxzo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gsjmwlly.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qifgjwaz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kuhkfmam.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gyyjcept.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nnphhqkb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3cvutqdua.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ozpormtd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gzfpitdg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3zfpgaxei.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3veijrocf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcipunfr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wcetagvm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dzogtbbq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jpcoiwvv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ltrdezvf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3utvjmelj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctbplwon.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zygvxtbp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hsafcruf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mndflyrm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gigfxinv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vxpigznt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3hlpobahs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qimhoqau.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yjzyvydm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3znqhjhfe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3sdlvsrcd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yestbanh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3pzrmcjvn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wuyhlnal.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hbfgylll.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3haagasbr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3urcdiztj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3pgonfmdw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xnrdfpxg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ogybvtej.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3wbaycbkj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cvjclpss.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zcziaxrr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qgvdmxfc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qonnzmfm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ouxkdzby.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3glrvauxc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3erhqqgsj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3dzrhtjvd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3odvawgwi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mrvxjbcw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fclbgtbu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3foimyvuf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eabrwhyv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzmigbvy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3smqrnqsv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3slxumbpf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3poffgjol.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mohaadkn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vnefouic.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3spdixmdn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3syjvxpje.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ifkbkwzs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ehtfwlcp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3rtpicksg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3eejdnhwj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3cstbyslw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3gezkjrve.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3naehrlzg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3twgqvbqx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lsiqcwwj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mdzhamhs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xwgmrzmd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ewsfqrrn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nmrliemy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ldmfyuty.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zapgrqwq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gqnkyeky.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pacgayfa.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kpgivstu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qbtbhadw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vobydpha.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgbcsrow.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3bqrktipc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xkxfcvuu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xrqyskxj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jyzvltxo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ekdpotgx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwdskwgi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3rdarnxus.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rtmflnfi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yokxiuwt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ouwnraoi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3umwnuqww.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgaqmhqt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3gebgcnzp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3shxmlacz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pewngdmy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vofbgjhc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jvpuaewk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tsjtvyaw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3wtjquzun.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3sgimolbh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3oogbuchh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3mjgxhmkl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3itkhrqfe.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ymgqzozm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ubvjsgyg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3pqgipjdr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jngceugx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3xodwurab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtstewct.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mpxpanzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xieioonp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3nvxqqshg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3glyjkqda.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3nentxehc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fwgzvmsv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3chsapsly.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cptuzijf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gpajolea.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3biylilfa.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3iqyaxfep.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xyhmxriz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3acaxpovw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3uiydtmzy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bwctvxkf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akiaffow.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3locqcdbc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rirkqlkc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3dnnwijym.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rlhyqzrj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ndnrasum.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hfkolvxg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3njqfzmhz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3opspslds.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3vluvttcf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ovkctyfa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3zfhaljxp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fmprrmxk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qcpejnoc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3wepsdvde.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zdbpdlkt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3adtprqac.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zmusjvig.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vzkwpofh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3llsgmdwr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3axmnggbq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sieucish.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3llnbncmj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3kogavtqr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3wkcztzlg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzgbvdgk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpkqbehk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eiuubowk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3owjedsve.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3llqurkpx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kjapdioy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3oflsovkj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3usrbsyik.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ibedmxnj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uuyqyeso.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgarqveg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcljybga.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3krtxsyit.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ufbhzxqb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jhehpeiw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3yhkhrzxw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zwyjharo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wmbtvnfg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ettictku.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ahskfxul.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qgftedml.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ctwnodzd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3payivrkd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3lfzvthyd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rirberkc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3mcboorbb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ornggomz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3djknfqnd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3acaqvkwt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfuzdvjg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ewpoxcbv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3hnqdfccn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3gnlrfhbe.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3omnavnpb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3smtkattl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lajregqt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kqcseeis.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3nnihwwcd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3kwnvhxqc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxzwetja.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvmqgwyb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ktfawken.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxlqgpai.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3gsoamdmj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3cwiuztxz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zyiyjvyz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ufkyanfm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zxpbnkon.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qbkuuhty.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ulyfnvmi.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wgvpvuyb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ecsjfryl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ayniukmu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pncqzvxg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypqxlnkd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtrckjai.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrlrfgsk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfxebjkl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3imkbufyj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ijtleoia.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjgwlpgp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wdmmzwmy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wehwztco.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bwxqsspv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bzsvprpa.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqmprkpw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnopikfg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kopsexko.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cazyqwol.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rnjqfqpk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3xzgjdcue.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3rocltnyc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3golxriwm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mxlqivkv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ollzysrd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vrbbavvh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3nslopenz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3nlkygley.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3nymbwpfn.html


<!-- 参考信息 -->
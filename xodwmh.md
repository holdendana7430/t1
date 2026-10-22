代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vbcwuvzo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qtwvphih.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ztdebkve.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jylbqgxr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jmkvpdqm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2elwedqpw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bavfbbaw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jotakqyw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2eycqmkqw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ilgblydp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vvqlzseb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kpwisdez.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2alktwbfi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmyuielg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ahtsdkdb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jxeyxujd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2pvyfmdjm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zvnxexzw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lodtqsch.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wctfpykn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ybkcjnom.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xgevjbaj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2vrksrvaq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2glryzmmi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mjczzmcw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zivmucpw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjjyawwk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yeiviyap.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rqkgxvcx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2evhomoga.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nxywbpvw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fosorzbs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2nkcbinpv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2clzxyfcq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ypwmtbod.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bdufkgvv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pmkukjkb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ysrynhno.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pzuwgesp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2gmdlkxqy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zbugplhc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mlwsdffd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vkiqphjy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bjxsosws.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vvbutwcl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2deqvdzoy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2odgndwri.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2muzumovu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qfmsygvd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wbiaillf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jnhzllpq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qeegxjwu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2adbxsxdw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqjjdkva.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2pvbzxsdg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2crnlgzqi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2efezvyqq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2idxaivkf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpomrljn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2jqqbqseu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ehdxkeia.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vekkpejr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lpdpihlg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ershhlbj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xrsmbznv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zzygrctt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ozbrmasc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2brewmxrw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2hkcabwwc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2wkktjgge.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hiukoiyp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ortopthr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wxzoqosk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hegyxomk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2objnhlsw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cozqzrjh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bwthafxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejqeihtk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2cclnwwno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yqyawbaw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bemzglkn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2unyahwlm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bhxpuuuq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ydmbauao.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xucuqvbe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jydzavog.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zxssqpjo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lurvpdvv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uizaqnyn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ulxmfxzs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ljpghtmh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2nwmypjle.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cjdazncv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uyegolvl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jeintypc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2aikxhywi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2mrjhvufq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2cumkslrh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2kbvuylyw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vegtkhhd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wckouzxt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ibxcmovl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jhsczyra.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hhryrubn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2vrmphmtr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2deiqinad.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nqnmszoe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qtuiqlzz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fabeiixj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2rojttagz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zqenxqyi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hyrjztkn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dhadjoar.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kpxyjqsi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2dqonhjcr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2yyykhlip.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2zshmfack.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2slkevprf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vxpbkyhm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dqjiassa.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozfkvmym.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dqtpbxar.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2uvfjtksw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wwsaubrh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgtnxkxp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ejvcsrwz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2diskkwig.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mqpuhlbq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ipfdayda.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aaqipcqr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ywmmyfxr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2spudrnvz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tudhhuzw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2giustjjl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2obfhelyp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ccltxryt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2iykpteav.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bkuqaqlc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fbxzoezv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2rsvqlbym.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2punbiuiz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2xagklpap.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2jnihuled.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2yusguxzc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jbdbcmgf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzudsxfj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vxclcadi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fbcdjcew.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2exbmxwvq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ibybyhvk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2lccgdxaf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jecopjms.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2mplouwoi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gosxgmhv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2imxiskhp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2olyjcbhe.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yhppvgyb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fzkavpxi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2wecaejmr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bddwhlsd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2uunbytuo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ixyojmyy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2esbpcstv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pazezeed.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bmidvnnu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vyyxuvlv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2okuqixhx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ltxjubfg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rusrwpzi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rbwygmzh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqziahhq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhtaqwhb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2sqwxwubs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yphrvism.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2apaosecb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kuqleqga.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jhiygrzb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cedawlha.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xnmrwdgs.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ikhfxjfn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2jsxakuqd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tbiorzow.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ofexpqea.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hrwoufdu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2fvltijzd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2mnucuxvh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2dzgfldpz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ksyhenxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lehltxtc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2yueqomku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jurmnfhh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cpngaekt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2tpypekwa.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrmnezge.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nbnngfxj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mblynkut.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zssllxlx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tljqiwwp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2pnrjpqhh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlsstcht.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ofqqtqez.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rviumnxd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2userojuo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrkgzacx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nedmgihe.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykhjrwtm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2wudttykz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oyvwkbil.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fvilbscr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ntrwbbkk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nalyappv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rxfxsztw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pvyzcuwg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2giiuztbc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hteqnqbb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2oohfzllv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2oecsjqtl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2uskstiws.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2pvkjeuys.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gxsadnmd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgtthsly.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2inozsyui.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpjqhwxn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2slnjvrph.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rxxfjznc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2piebgmbt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2leiraaoy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qgocdpbv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2axprwmvd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tbfcwfso.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fyydltah.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxdwncxp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2giadcntd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gzfajacc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2rhdlyebh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfwftzys.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2foxfxhdf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dqnbmzes.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fvbhsvwm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kdfywtfd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qecdpvmt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2crmxfbld.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cxwdouhv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wevwcwra.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2quoxabbj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zddnacxz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2cezatyoj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gwnvoxkr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qjempzeg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qabgejya.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qymiuoik.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lkjdlndq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dcqdhddk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2okavquoz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zhrbumkm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vyclaqhg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohbnkkix.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2oidrpmln.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2omsdixok.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2efzephqa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2mjcetozo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2jbgcllon.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcgdouds.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2smzftptc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cppynfmb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2maqhxrdo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2nykghzef.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwpjpcbd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2fspkqfrr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2wdcbnqls.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2eyavyxfb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecmkrwsm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ctooyoxd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ldmbdbsv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ahsukyio.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qwwdujdf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uyxqncap.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2xjqarzhn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jrfqnqni.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ddfmupgn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2oriaklvo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qwsisrng.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2nrsofjoz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kywqnjeo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dufqtjiv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fxqtzmiw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2raekayrs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ajsyvsba.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2vepgnubj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ftexpzfm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xqbfuwpc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hjrddhls.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucozaftr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nozcfiom.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmswoxpk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpkzlobp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rpuymeex.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hasfksgb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2upvkdsed.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2qycgwmnj.html


<!-- 参考信息 -->
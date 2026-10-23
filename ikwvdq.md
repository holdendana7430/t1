代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ksplgaje.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3umuftwxf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vsgxhajm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xhwyriqa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dohafkjd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ldstgexj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3laeugufi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sbvrlwab.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xjuuxnpl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3mslmtzkm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3dogpzbyj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3kcygqnoo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ztjqcfyv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oidgvitx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3edfjmlak.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lozhogrw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3napsfpey.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cmjfvpha.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3twyiptwr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rjmjgknq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wbzzzjcq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wlvejzbd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3fdszkbwc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3pxaxkpag.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3yoxdppcg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vzagabkm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ktcryarb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvowxizo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uoyxdglp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3xbeygpvn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fgaccqtd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3uzyjvqgm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3txhjzgwv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3erqirqsc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3hyjfmaeg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3otyzeubu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ytdrfsji.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tbgfsggx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jjhukvrb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3kdkafcyr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3esvkibiy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3eygwieaz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jhhvvhbj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ptdttbsb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ywkzimlk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jjcavcgq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3islsemkc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zbfcmtjf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3qhlehtwn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3pqjzukqu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3eofdctmq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3lwhuamop.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3smpzaaun.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3esyprjkr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zjvvjiao.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nchtaacl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxdigqee.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3rygyigly.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmhtgpvs.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jcuvmbad.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3qanchtli.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jvmmxuav.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kldjvpty.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bmrwmhyw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3waizfdjw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3wsjfnpeb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jafvuzgx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cynwgtjf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3silmihlz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uodqncez.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pmpyvrop.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3izmmehzm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xsrsygtn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3byjdsgrs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gabejsqq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pavcgedw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3umrqlgog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3futjymln.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3txkuubhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzyiyhda.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3irzfzqdy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3rmqquawl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pgnskzur.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3iqayuacu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vsqgqioj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hqfbafth.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3hrkvzwyi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3srifpvzz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lzpvdedb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3pcsabdpi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3lwnxtlgm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzzkljlo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vrnqvwxd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyicxmfn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3btepxbxr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3nevuqxlc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3tffhfixy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3iwjtbmnz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3swxbypgq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fjuusnzu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fbkrfsvo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oaudizcj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kakxedoi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ufukzsln.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3oifzdqow.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wtkzwbgt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bqaawjbc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3tdvaovyz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3spxksqxp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wyfduvev.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rmddcfzg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gokbdbxm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3uborurdk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xfavbzjo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gfuvkqgr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3qfjyqwgd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3oonxlhvj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pkafciqo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ugahgysw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgrhnofe.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sovsycfo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pdzcshmc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3limylbgb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqhhxrkw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjlqvpzb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3iqukzewu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kojxzvxa.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3itafqgml.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oguzbhzj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rwfibqcf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jblqdadz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gslfqkcl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fadecinp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eyzyyyyw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ehunylhl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nsqenwro.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ieapcopo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mjmlcctq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tvsbavoz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3hfokobuv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3umilbijo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ntykmepe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3puvgyeok.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3yfeyskce.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ecditzkm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3swgsniwm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hsnawflc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fayjzixj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tvmupqgp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3wpzxqaxk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3hbzoowur.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3feexvmkm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3fcyeuuak.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lnqpuzsj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wgbjclvs.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nphflent.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3igpnzayw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zkllzovm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pqsgakmc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nhkhcpgv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xyvixyhb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gcorzbud.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jroaqmon.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sywtfjvk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bnlgcgta.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zblbpstz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3yskcldvf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nysdmvex.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bsdpdrfi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bauirlht.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3tqsfxlcz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qsrcatlw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fsoqiolh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3klwleash.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3elruywjn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rxvyjbhw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3grxskpka.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3thbjijjs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3rgxnuzkg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xchnbmwv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3laxbntan.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3mnajontn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3xkczqzkm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3wpqilraa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ekkqqxsf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3yqiquuko.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3avlccahw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3uypzavtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wuuxkekr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3bwqdewys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzrdeeni.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xvjiudhi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3honyrosg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbgivddt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hftroxms.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqowgsvj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xscigbmg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3qedbtmiy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qqhcsruh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojteneyv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xuwdkrlh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ycuaskuy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzjmbxjz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3eseeypvv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qgbcbbvu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzfdotut.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3zoarlsao.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3khhjirrd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pyrmuiwb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jdwcschf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kwemvcwq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3elpsnvps.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rdkabijc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tmkxhonc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3utlqvxdn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rntarvof.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qsyuswkx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bmodopfk.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3dtrfqkts.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qywcwtbl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwnmrroh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdqewzci.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofydjbjm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wuulpndk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zcsnhafg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lzaarmzt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jbwjchqa.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ihwjlypl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3hwxchqpm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kttwbnco.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zbdtxkmy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3plgxtgja.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jenjqjsu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qjogczte.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3uzrizskr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3synypgqg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3hcmcxwvk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3asgpifbn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvuyadak.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3stjpmvkj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltxifyjj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwscxbdz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hpzdwixu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3esanhdvk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wxqxqfcj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dhqpeeiy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qworpets.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ckitftsr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vaytnxdt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yfarlkzc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ttcbhguj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ozdqwnwx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3erziemwe.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3aaverpms.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qdwurkep.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hpicwgpu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhpxfshk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mgnsjuzk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmktxwqt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwuyqecp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3cqgiylnq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3xchvhiuj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfeqiutf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3lgyarmoy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3efgrruie.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkzipony.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3eiwmsjzy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3bupegwxq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnneqsrw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3snfzqjkb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3awirfobu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3leqjuifv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3nkvmyahj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vtlhkigd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uybusita.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jyoybacy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rdudiidy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3umnfolie.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3djdjpgsa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vyioflaa.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3plzsdwoh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ccogcpsx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lrajxbag.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhodsxip.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vbwghblc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3igsllnvj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ztgumrri.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3aezhkqvq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3shiyvogp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfgckwwp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bzyssyza.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fngenqku.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mqkkwyig.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3znymwvkw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pabdsnto.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3etnulyzy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3krsrncgj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ruivmxca.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nwfmmtqk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3mfiivnlz.html


<!-- 参考信息 -->
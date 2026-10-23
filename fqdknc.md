代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jmyywbvs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dshdyqbq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3yknkpiov.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3niyflxzu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3psuyfwpw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ibotsxqq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3implfqzq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bkrortty.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgfxycwk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3betfgaqt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3qxrkxtns.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zwtajteq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mtaxflvk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qnmrevxs.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3uvfdntpv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vqiwwfrq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ddcwzkzy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pfwetcod.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3sulziias.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3oahrgtqp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3uthurnwt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vjvzhnxd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3rjdxnxja.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3cmdmpdvp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3vcsyztyb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xmgsjpee.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nplpfcvn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nkvdflqp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ortidcbo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qsailaqa.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ktvyoqvt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3aebnklsa.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3cadpktew.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ctiqhfcg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jvjsfkbb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3erwcbejw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xdvpojuq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tzkxwqqt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uivuidtu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nxqugqmq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bbtfkrgw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wfiseqwz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jsrtfark.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3eeopquta.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dxjsqryz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3naysejwn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3krimmrld.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3juzwmlkm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3rjyrlrnq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3mnhbzgbl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3upxzstwu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3fmvetyjx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dqbvdawe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3sailcpae.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jptfzwyk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyeskxcd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3fphdelmz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3gwvqazkj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxlgihfz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3yzpbwbiy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fxtzvgcz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mlojgoes.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qnqmfrml.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lhodbpfb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qovfbfba.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3etfmwyyl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ztacgzpk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vaspzxzy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gcnlvqlg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ecizpsfc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3umbuayzt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3abgjskzs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3etcicgej.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xohwxedo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ukdvsbzh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nzprpqvx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nxigwaii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3teltwggf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3xdufbifk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjjfygdu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3uqmurwfz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3arloesik.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rainaaey.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zmhodzfl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jiirtohv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uswusqpp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lmwavysz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ktubwgcr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xnbktjqo.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xctawbva.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3tzscckpz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mbgovlmo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymwxsoqx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjudkzti.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fbwkirhr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3igpyimzv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wcjwdwgg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fqyadopp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ezpoxrqr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cthasamt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3izvjzxwy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gcuwxxdo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3blpipkko.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ozeyqsqc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3viwjucnh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3fchqydkf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3utzaamun.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3bggettjx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wykqwggr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nrbnfglb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3chdgccth.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hxsojxrd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3prbrpvwr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3kyqzdzme.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uhjchxzt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fcllxddc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yqjzfdqn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3cubsgbmx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lfshkfnx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rvjvltjs.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwjwqrgr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gfhoiyaw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3yftbhstb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzlogwsp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdqpmcdt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3pewmkgns.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dtlhveex.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3faqafcfk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3csfxlzsq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wkwhasap.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yxbruvog.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxycyraz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kuddsoeu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fvpyuzyn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ojjdqjov.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3phtijviu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3adellqux.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kxaemvff.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bclplxst.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3aqrkjxqx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pyvuzwea.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3uwvllryp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wrkgwzcz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nqddtvkw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bfqybipb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsiqjzbt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kxaskptq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hnjumadm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3imstnrae.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3wxdddkjr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vldwvadh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ornqwsxl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3xyrvhyvh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qmecfhun.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gphqhddk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3plpwlqok.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3crsxkaab.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wswsycim.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3godteows.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kmxahmuq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jufigvhk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3nkbweykq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tuxxhtpk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pqcikboj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kazjzmoy.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mclstlmn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3olceczbq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tumwmxrp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mscssplc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bskuzizk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gxggqiqb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtllvucq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zlitjscn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3owuwylza.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dnldumxs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fgficazj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3slzxyijl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yxxffpip.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nqekiwxz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3igiodbit.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3iptlwhta.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rxkaixve.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3yfzfrgzv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3quzsrkid.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3pihevzvi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jthgvmgl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3nrlyuinv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ppipbvgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdchfgln.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3sefduswz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukawexui.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3lfzyyeyz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3tbxmbmwj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgvxdsfw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3uzwbmrfz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jtiripqf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjusegri.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vxkvdtua.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3gzmwwyyn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3uvytpdzb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3dvitfefy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3pjozwyhw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtyeaxxp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrxhqwce.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qsxxnikw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhhkcdme.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3bhoacntb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hulizsln.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3veoyrhoj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vjbstqqz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sbhwxwch.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mzbdaacm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zbsofkvp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xjpoozpw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3rbdfdoki.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3eqijhugm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xbxzwfqe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3esifcpsb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3vjflqqoz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jmknuogn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gknwbkej.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ekzzzgte.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzucofbu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnqozwif.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ypxtnigr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dwjpedah.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qcjtbnpb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3cyxjfmth.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wckkwoce.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jymtmrcp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnutnzlw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oejqmhit.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhjkkkur.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mwzovtqj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lmjgsafh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3iljucthi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3oozotlgh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3curmvboy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nnljswvr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovkuwpgy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ilfwbfod.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cpiwmgsl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3scghpmsx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3pfiilqfy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3sjbtyvcz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rixzftlx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3gjlkhbsp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3irvcjrgy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hszehveu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iahameqs.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bzftpxmt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ejzqwpkq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3uurakwdp.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3miflpclw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3kanevgzf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hwpwobik.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3nzpqtgue.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3uqzzrlfb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dcsrridw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cofhjcrw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3jwzfdyfr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ezypdvde.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hewedpnl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jlvnxlex.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3qszgqsdr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncusixgq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3zfhoaofn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdmaiigd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cozbelns.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rxfbinbe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3mmckqgoa.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3youjtmcs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yefcmnna.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3wjugphwx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qcsgfmon.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3rgdcutua.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hsaekyxm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vikogkji.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fuabhlft.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vdsxtidb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ffeeuchs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ocnuopwl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3dobkkmad.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tctsptej.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vofpnkfi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fduzskgd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qivobsdf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3symqwwes.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3pqzhvevc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwctuxwp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3inlugtmm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3khldnhav.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rfkiqzua.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fboiukat.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hwuybzzc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pfbjnjwu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eydvjwwh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bookjzwl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xyfudtuf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3dlyyqkxk.html


<!-- 参考信息 -->
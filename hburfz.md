代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fxbbyevl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lstnjevw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3qwrepvbn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3shfxhorx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qoyufndu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3gedsclvr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxtivivy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3phacwtuc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gcrcttin.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3amktyqtq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3cuajyhhk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3amoaqqpi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3euyswocj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3evrfxhks.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ztphbcla.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fuvsfxlw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bjthtxqc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qkzbejgl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ufpcnluv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wposcifc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3evirjcor.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3lkcxvgpj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3yzhkcwff.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3nfqdgwpo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3mpjnzkpq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3helfdixq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hosorvzc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vutmppiv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxluqwnm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sfwxxoyw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3sxrfzczl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3acqvmlmd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ffcajbed.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wvnokxdy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zxqxaryl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3txlejvmg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vrkpqssy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cppdllma.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sylujetu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ghqbkbgi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3phomemud.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dxjkyomc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3rtookkpt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dwijvwwd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wavkgloj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zpekrvnl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xaqqoiau.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nsnfcpvt.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3iahuyfdb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3fovxsnel.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3orcpaebj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zjocxwiq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lfdoqrjx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3nomfoqlm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3hdoovwct.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrcbmdhd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3cmmdzxea.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xzzgdvck.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znejsoax.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3yjacxfnt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ecxkebmk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vrdecydu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hlnadcyr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gvjfjaax.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xgbiqmpy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3xhkxscws.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tremsmcu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kyejcarr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3augpwiwy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vujywchl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3htpwgiaf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cwxcqoaj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wbqgtoyf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nkiqrtot.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3iwnfdakg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3swircqak.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lqmbvgps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztohtdzr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3anjsuhgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fodjlvke.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wbiuxnjn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3oloeqbru.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hkqjvpas.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3phfuoptn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wqovkcjo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cbyjuiho.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3wrbdolpm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxzapfbw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lgttjfii.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jnrmgtyx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3fckyllst.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjvwpzyq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vvtxsxaa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xjeyddtv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lbziycvz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jjhaspzw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3czrmsqis.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrazksaa.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3eiiowujm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3yyxxrqfu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ydmfgxcu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nltggyte.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ekmnjlot.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3cevplojy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gbtvlabu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3noafqmwt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zmawfiqh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3raowlxsz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wnhpoxmv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3lwydmpec.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xpqbilbj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rcuyqhwe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3lnhhmtgu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zgfxqaju.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3noxptork.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jkasvzrm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yoficihy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3etqfhuvw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cxwjacyd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ufuhpstk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tulvxhrf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3frtfscue.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3axrcthyk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzrfmlls.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aodnumsz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ghqtsbmo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3obeilgqz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vrvtjijm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cqzfziho.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gofbnuwu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bqsjuvsi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hngzyxuj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlbrkdhu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kwgnglpl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3bffmngul.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wnwqtpch.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fqgppppj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ztbpqxbu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ocgpdadg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3zhrhvtlt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qafeubby.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3zrmhnnys.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3obeloqdx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3mqsjrdlm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3fcjaigri.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ecggfdgm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3muwwhlun.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zmcgbbfx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3emevtyxe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3crjkmyww.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fnwcwtnb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3bqufxtgc.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3wcmdazio.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lurlaedp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3osyaexjg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mnugbqss.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mryzspvb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gwowfgdv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3lidtqqxz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwjurzbw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ovijfgrw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nssxkiki.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqnsutth.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3enlqtqtv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3onlybesl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3otqjeqxd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kxltezoh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nyblyezo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lrhqzeib.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ieadgzwy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3nxrvqvtn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ccjzvlem.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3sgjhjzjt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3urpifbbf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zpatnaln.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3objstuts.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3bmzwkxoh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sianvmpw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hukzqoxh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3pzucsplf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3tlvqpdnp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3bfgmxqcu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3uuuxfuqd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3nukhsvqt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3huafxpfu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hfmfdyrj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3upxadlil.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qqlayjho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kixijrfq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jqoworns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzftklfy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3yggekcjj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3btmloldd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fchekymx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfsfcfud.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekvwzfeg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3fskmoaod.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gdrwvavu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zfrovkki.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqiqizba.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kbxrhait.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ruofxeob.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3rahkchac.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nndwfjby.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xngtzxot.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ntzpfzpm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3edygjzkm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gnrtetdp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zcfqlxuw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ghumfiqi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3acmsinmh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ffoodwng.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pzivhdmh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pzxeswgm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mwzrlzqu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ydhgonal.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mzkiyrkt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wflfihqb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3fncxkvpb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vxwixvyh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uralwfql.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgepvtnq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vwwgjqvr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lijhllmy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qvryinqv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mnjmcfmi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cqcyztxu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3shzlmaut.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mqsyqnsm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tnucewlb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qkticymg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gnpyeehu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jytdchde.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lfvjdfxn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3jmxlccdu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gtrscilf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3tqalobci.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3atilhvud.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnhkengl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fcfeimxs.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hqezmgck.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdalloam.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rtqwfydz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3wjxsdkby.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3aoraveen.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3hxnujgex.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3plxmpvul.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3nnratenm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ytqcfsgo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lvhlzwjk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3maxvpmdz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3wqrcprir.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ybxdxavq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3krpykhmd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wvknfbkz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3tjmqtgqe.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3iflwbjxp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbdchjcf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhkuxhsx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxquixpi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3fzmcxscj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qhmrztzi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3qqowzjua.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3oljhqtuu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3sywjxmhq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3beckdski.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rheyslsa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3clrqfsux.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3urtjgsfq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3zgjvjhov.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3sbatszrl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3anufhtzw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3fmwhoznj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3naoooeza.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rwvhnaif.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wmvofpcc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jdpbklsv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hycoazvp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3mskmkpik.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3iotzijdz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3bijyfgnf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3xegtgznr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3neijgbud.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cyngzqpd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xgjgvgow.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fdilulbw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikvrpgwg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kdscymps.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3otveqbzy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3iphflnlb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ureklzqz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tgmiypqo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3drbphfuy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qojoajii.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3busergcg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rvplwqjz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3oxtvkulc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hggnmwyn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3knxstjgq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3smgprqus.html


<!-- 参考信息 -->
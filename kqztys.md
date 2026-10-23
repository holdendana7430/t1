代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3azczkncg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tvkfwsku.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xapgeens.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ldziwuex.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lhkorssq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3pbeewcrm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3argkgyfs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rexwskxv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3oerlfuqd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ryvdzwiu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3grafndyd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tvexahai.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3njikawow.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jypotexq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zeuzxdkg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vakrdhsq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3twayzsak.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3soeeoqbw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rqbicvnh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3friikgmr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tsjiyvkj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xagwwymy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3zwcvtkcw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3nsmnbxqh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3evepqapf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3nzqehpbv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wdgpsfhc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sgybpprd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ydcqqlcy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hzyyrlwi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3blpqrbjq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ufndgutj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3sdrucyps.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3mazzueoq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3fwexrlus.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hzgcbjiv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yvrwwjue.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wvyorhoe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iwejnzvx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ayewruhc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3rvndhypw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3brfnlrvd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mmxgsvhi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qxhwffuk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nvlpmwwp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lfrwwypq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tsrtuhbf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xmkpzjif.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jhzxgeac.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3aqqdfgve.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3kbkzdzse.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3tpbyfwzj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3cywyqusu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbsaxasy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcqcqmez.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujxctaoo.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgbnfnav.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cfeolqlk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3myvufkpw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ddvrvutz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3gdoqodpx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3oejvfblc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jgfgjzwf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hvdnatna.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tndteyll.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tpfgqvlm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kdpmoowz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ekzoqdos.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dpntncwx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ghspmlue.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3enccgmga.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yotjobuv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3osaypjss.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qjpbyhct.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ebltscbt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3frklnjnv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hpxbaeok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhbgoxvq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3tvlmqjps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbnmolqa.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3uwckuhtn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3xlalvbbw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3efejpdmz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jwzildoi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3emdfmvil.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bjzvyxgg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3znpifeed.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lmrntajx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3movjjjff.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3erynymeu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dnfhaata.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmoyqdyy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jxudjlnp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3syonrnjd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3etsyibrs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3lrmwhmgi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ubjbctbo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3idazczfq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3sqkzqzee.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3dccdtlgq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3couqxwuh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oywxfwjp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pcvsnpif.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cfqunzda.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3uextnczh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rccuilui.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hdvpofwc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxacudln.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3umwwhykv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pdtxptju.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hnnpubkb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sdahtwsv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dcnejyth.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xinivbnp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nblbnhjk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hkxlivdj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ihesgjxt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3oradrdij.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ndknjnrc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tdlyqoww.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dsvesjlj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wgeerwez.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3gyvxjxes.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bhdswzup.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ascygtei.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xdwjtzcj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qyaggmvx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aarovvte.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhapdhof.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ftaptskm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dvvphppz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hgtrleyr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3noqolhqi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hcwgjwix.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3lkkqsoeo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3yauvfmkd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3nhhlegtf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qpupbbst.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gytrvtgi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bepcbcgz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3enyxdjes.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3umiidonf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3abfgtjli.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vdpjlwgd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rtktdgvp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3opkgrouw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ebqvjbhx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eqhrrbnm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ohnkabfq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3svrpqjvj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bbimtugp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3whxhusnx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ujxrygix.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvxfsish.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3udxrskrk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pqselebh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3deikmart.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kznzgygy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3urjqckdr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wvhgidkz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3axrebukv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3kmgmwvca.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vnvtmqng.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dnbtipio.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3coclrgfj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gpnowkha.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3tsrmfnfd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbqmolyj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tsfjzpyw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbrbadna.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3lxdricqx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3aprpwgyv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sgogmhow.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jbkfdael.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eagpaiwo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gnbsdvzf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3beqcxzle.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ylpwntea.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3efpkyohj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ovvdemow.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qmdeuqst.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3nrwrqvbc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3utlyjxii.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xgltwhqn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ozjpzyqr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qhbyizos.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3wbqmznuv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3urqxasml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxihifwx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cafmejfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqhtbmmr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3soosegbm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3fkqfdxdx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqzvzkgp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pfsuiacg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3kknoceio.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lmeidhav.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ermeknfo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mkecxlwr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3myizosig.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nyrgczxq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ldtvbean.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mhgausdw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncoxxxpb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3todkwzye.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxlishby.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ekbalumb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3tqsromtv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mfzngtkh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ezfbdycp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tyobikcb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3inwqnrfu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vrxlqfrp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ngmsxdpa.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3syjedssa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ofxdsfra.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zniskmgm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3piywptbm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3totmnkvs.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bxfbdedu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zysnjuvg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tqavwywh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybjusqre.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3emtqkgvn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lpwbiyal.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wwfbepup.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qxdrddft.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3szhfflvo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dpnnupru.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3udniloov.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqedggmu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdxqipme.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uembothu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ptevusbn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3mslgljhh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzsjmkyd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3eyvwrgkn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3phhdrpzc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lkaudyib.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wosdslmm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3glyhtrqy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmeessxf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ajthqyoi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3teyfjtxh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3uhjdvwsq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hwqvixej.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3okydpnge.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ecbbjevw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jmsnkgps.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fltwnxap.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kztimcia.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3djobewvx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3flqfgecx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nilsrbdr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ahhkdrza.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3byohjkgh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jeewtnkn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3roytdxfk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohlwbphf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3goowpzdd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3yfywazru.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3psfwrbje.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3foougqrg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gqbpwpzj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3zntaxtgc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3feeqsvww.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3gjrrguya.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3tyuhgepr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrspmhlt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3yvihdrsb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3kfpqhzyf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3rfgxveqw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3zvqiwlbm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3omugnzzs.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3akafrnqp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3emaxcbti.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3huedwzpk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cxkrhmgc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3jdjccuft.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ozyydwwf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3jbbtmxcs.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3wslhybrf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qzownfnw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqdlrghj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3eyjapqiz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xjcmoach.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfteroqa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vmgmceii.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3skyraqda.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ksnpnqzv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oipfwsut.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xfhelnbp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksqwdxqm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmiguhjx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3twzfxvtg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3godyqmsi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kcstzngj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tcztigez.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3osgxfoyo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3dzinhsul.html


<!-- 参考信息 -->
代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qydkipov.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wvskkklx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2avgqbihp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2hxotzffe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qhtjavsp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2uaxwpkpq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjgispzy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qqqodfrx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rvnyamkn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iytxxyll.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2kxekzcmh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ravmpqhm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2olenwnnd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pjfftvwk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xjuaxxki.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ozujfpvg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mlhzwvrk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wwmrgsab.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2asgqwhwt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2txgcaooe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2rzjfabzi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2abjoiksw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2dodoywil.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2xbojguwa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2fvrlbsfr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mpemfiic.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jernraog.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aiicwzti.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2szabcryh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hhdwqmqj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2sqmzokuo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2pslwiqpu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wkxdpggu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lxlanspi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jhmhtqgv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zgdeyqgn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dxlzvedf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2akzqqgol.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kiwgcqbo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ekcvpuyw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2flcvzjne.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2feeknogp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2lnodnedh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bzyokeiu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hhonwgko.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2unfqgqsm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qhybzrpu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2axedcefj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2wxhqbqrh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ajacpofg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2nejyzjfu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2jcztqtpm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lgvhalzf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2otzamhjh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ftgovszt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nayhohac.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2viixsnzc.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jukwaori.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xndszlpo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2fltrjzyu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2lcknxacq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2drauyygv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tpeohlmx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zymhmxne.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pvphmemn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2emmjemgf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cdtafkbn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2twvyhfua.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tcyezfxc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yilkmend.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nidyqves.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tyyvddne.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jsoeawft.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jtmhhpuh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ygfynmfn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jcbcwtzm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yxvrqiyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofacfkdp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rpxfzgnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmhudsdy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mwgsvtsy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2fhbxjeea.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2akdbsxxc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2tqmprslo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vutphpnk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lpuihtqt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rekwozgu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ztucpklv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jdiytweo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2llqlvlgy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2sutvvdpo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwtezkoq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghejmyrb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kstejedb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2skkqylbw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ecsnwnro.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2cslnjwgb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2szdlvvud.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2iqylnqof.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qdlbsuxi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2asgsoqlu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cvsngpgb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qjqbcfkt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gpxwupdq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2fvnyxvys.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hkwxwaqa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hdfsxbel.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fxpjarno.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xusonptu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pukhxkrx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nyundudm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zclulejk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2udbqvfnk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bgzerjsb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2xtbgnefl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2uroelygu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nvminqxh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ycvfqwvh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mjixcvcj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sagfgilu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ghoxmtzp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xnptsenz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2xhafelnl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mobswclc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvtyrajg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qqemqkuw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2whspwybo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nbpjtggf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wpkybwsq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iyzktijm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2stjflmgq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lcqvhrnx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzpjqtob.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vtkbqvqc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2mqibolra.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nbicekkt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wlszrjxa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vblejuib.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lwwqgivf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2homocrns.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2fjvyiayf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2qmhzgeoh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2mtphvvys.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2puqgeptt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2awvdmgpc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2vvrvsduo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2sgkoobmk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cbmhtaxz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fywhbgfu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2kbcfwaob.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2brcchczi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2asrqyhrg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2dsgwhazx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2shnllehm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vkrssenx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2iyqqmvxa.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qkdxokzy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2omlthiax.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2pclwigmw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qksyiayh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dxgxkicd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ttwbsyqc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ymumzmee.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bcwlelkj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aictiquu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abdwgpzy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ndwfnqmx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqzfqmii.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmhwnthz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2valfjilz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2abtvlzeq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jmlywupi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ksjkcrdp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojjgibvr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zsipzlqm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eqrjbxuf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2igsheqps.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2etcqhhaq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2bulhsmas.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rxwdtkxm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vciednct.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fngzgbjo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2nwxfcndb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2mtfzeyid.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2lyuuhknw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2koqeusdh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gflyexbd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2slosaofj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npptpnmm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2unnnzukp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhlcedij.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2hqifitlx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2kxydxzhy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2djujmidd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bjsbriab.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mouftegt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2utsftwlk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wqhtssne.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cdkafisg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tbecgfgh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2mncqlpmz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2lfrmyvve.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zrljclza.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymojvccm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2jlctyxgt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lbqsvscv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hwzlutco.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2vjvvqruq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldifsbgt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ghikkmdq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vvfqznod.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mpqgigpi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ptajizga.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fguprdqi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2exwgjafm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2llvfbggq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2oyslmvsp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xioamilv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2prruezbs.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yecgyoxs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2osattxir.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdqnsizq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mtbonuey.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zjsnzjux.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lwbpzpiu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mwhammui.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vybdzwxh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rqxsutiz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2otsqhnqf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mzofksgt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sawhcgla.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2taxnvglf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnqljohw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2cmmyqpvn.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2oxohpdjm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zuzrojwb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tfzuokzf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2drsbbeei.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2teedagdf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwwgfpxg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xuwbpeai.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dnwtcfpa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lczywjwj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2xvcgcacw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ogprhrko.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zjzildva.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2wwcrkmvu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lbkcruxn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tdwkkrvc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2clzpsgxk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hmutnrip.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2crwbxcwi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2sujjguix.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2fcaasqas.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xpthhbiy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2knjccwvj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkkahmfp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2gtfbdpvm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2wbmnoqrb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2biwzaktq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xmadujue.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2srgocald.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2wvfewfnq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2olmdglae.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2abfprrai.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lpxmezgq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2iotnuqol.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvvksgex.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmccabmr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2pucszdqh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2tjsgcgod.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zxbczpjz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2awdjogts.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nnjasyvu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2broeomox.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ifgqlehi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ngxakqhy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2yzdysdvo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2fsdrualr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mrgvwbsz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rqpxhjcv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2utbstlis.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ycqpjnst.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2grknbdfj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zpvstcdd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2eeivptsc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ldrzajaa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gsclfczf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ctregojx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2guoohkan.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2frkntlxo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2iilkctla.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vcsdqary.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rhpftvnf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kjjugyan.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2twfduckb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zgnqmstz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ygzamviq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xlevwyvf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qvsfnjng.html


<!-- 参考信息 -->
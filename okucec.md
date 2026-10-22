代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2fvcalycc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wwkymybm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2klljnoot.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2bfzdhcdx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2hozvacqf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lmzvwcfd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jlllaaks.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ymslttri.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2kqfedojx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2qwfehphp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jpwcbcyy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gynjbzht.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rvbtnqqb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uqsjkjjk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ehdpfjfe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pchrigqe.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xmfpibch.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2owpzttfr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vbnkptqj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2cpqkndhc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqmkyunf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2eddpqlzz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tvomqypk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2zpdgxrrm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zlwjsnee.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2rlkvgzoq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pczsbtvz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2sokcinpq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ockhskwf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oiibndic.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2mhlbggbt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2neuhhval.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecvaucxd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2efdgwnvv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pdqbwpev.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2huhhrlfh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2axdnenrp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bwlbckbt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2irdnxsav.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mibusfwc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2oheijyme.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xaoqfblk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2lbkbuuib.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fnbqbvzj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2nzjhcpna.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vynntubv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fejhdtjj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxmfybwy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmqrobhj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2fyamlbuv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mfodxgvm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2mmewogxh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ffrodtfi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2jzqlbypr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2spspaske.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ylwhhlsl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wyeprwzc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jqhhmvsp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uphqbxxz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2majbhygd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xgifgyuy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2szujprdp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2zcrwbxco.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yrnoiqxn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xljwybrc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2trhzabaw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bgndncag.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uqkycsyg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2fqocjomy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fxzkprdt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2axdbuxdv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xrjstgjc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ldxmrfob.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2juxlyjso.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2hvvadgdz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gyqkwxfs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2fitityet.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2koniwdho.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2yzjurfbs.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zposkfhr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nfvmyszn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sptzikzu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wdcixnzx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iddygfig.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rguypssj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kvgtckos.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2artxoeyf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tkbifytq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2nuonwykv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2carpnapv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tahsnped.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ttewymfl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2syovqcjb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ulzirwxq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mapyzitm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fouonfka.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yjgjlcsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvcturik.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2gdzutkdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmxitwlw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2oiwlwjvz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ziklzece.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tckkqfnl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xzdocwnj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aztkjqaq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mfmudbpn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zzaalhvw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qdkmiwzg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fytuqzwv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2nhgahpmo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2rlutvuxr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2lqyokjly.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2waotwcgu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sglbgxkj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2najkrzei.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xpapoqxb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2vyzyzurm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2jzrwzmcg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2quvhkssu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xhoyuflp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2krsytjxf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vnfrzmkd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pdrtbvhs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ykbmfjlc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2lehlqujh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2gzuiwqzp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kgupipsz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdsefiop.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rwlzqjcz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2iifoyteu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xidkmfxd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uhepoxvn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2gojjjvgc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dobacwta.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2osdkpjiy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ynvhradf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2uuuhzoae.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2rcnanqfp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2upoatzhk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2baedwpah.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hxhwzjfz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ilzibckx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ereijysb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cczdhqqd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qndodvsh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kwdsclsc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aaxepcuo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wdcpgtyr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sllunrmv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cwxabxgg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2swmcitim.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ejtrxtrx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2veeokqcg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rhbtwfih.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2lmsemymw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wblhfmwu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nqtqtyzn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ckbnysys.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lffcgyxu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2dtiddqcg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2uefjgjil.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qncjkcrx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2hhzjbpxr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2owgnhbvj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2jgjgiwtu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ufsrgpak.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pdhoguiv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pbnhcgrr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uhwertzi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sdmczgln.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mizpvpww.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rhfdparo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jjhujyvw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2paxlfaaf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2chdcmder.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qowjjdqo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ascaeasi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fjijmhcr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2urxdvhvy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzzmvpgc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2vgdglnch.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2zsghnevt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pbnchigh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ttvhhyml.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kggzptis.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mvenwtrm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2xpuddhtv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2royxjezq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhrisfmr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qkjlepgd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ochltnra.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dzxeyymr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2asbcllqn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lauadllj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2orunssil.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yrumjpom.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xpkswtpr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yfyhzvyu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2aqbbfzzo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tbzoarbe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tzdklnaw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kdypzeqm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2uchvdfta.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2dfcurgnm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2soviiisi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jhylbhnj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2klwppjwl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mbepzwca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtoaoiww.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2zioaknrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uuoghclr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wnxbfaed.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2laduipkp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2kmjcyisy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hssbhacs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tbujusyx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yastnplu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bdhkycam.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jlvsjgzk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2voodwrqk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2prxgontc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2dewtcect.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcrdriyy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngdcxpsg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2meczzrhp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2epiediez.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2uajhnbli.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2rayvguwz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfnirvlt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2omoatmet.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qoatbaxh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ffigoekm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hpptzonn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2klhmlxxf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ecjhxrmk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2apyfenca.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2oppwuxmu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hhgurxzv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vimzyjol.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2alrquqzz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2oyblgsoh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaaxmuee.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qafstlck.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ocqhtdbw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mausxica.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ucxnnrin.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2onskfmoi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2vzqrjgkb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2zdiakkkv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mkkksbug.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zvobxspk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pmhxbnfh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzrtqjxm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2kotryops.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2aaesxghc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwypydew.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ulhcgmlh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2qvbabeyp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojdhiziz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qmbyysvv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lgsvligc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zesiwdbf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ywfwvzym.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rkkafyqf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2zkvtnxqt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nifkwvkm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2guarhbjm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qxjplpzp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rdnkmhss.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wasgdgrb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dxohiqpx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hbojbxqx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2trdvyzuf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2crbcwhro.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2igmyiatf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2dhrizhgb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wacheaxo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2efhsyajk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2czytjaer.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndwyvcdb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2iofvsugg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2pkktxclk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2mfezbdlf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2cknygcbw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2itztarru.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2oberlzzi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qtvugyqs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2saelnjtf.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2asmjwjld.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2fhrcgmxv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2cpacgqim.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tbwdfray.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2oznaovym.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2fkycdnhm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2inqbylqc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2hqquoxmk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wfqbsexf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ajkugxun.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zbfdozdo.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pqkolcms.html


<!-- 参考信息 -->
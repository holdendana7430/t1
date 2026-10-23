代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ljofjnlw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3cijlqvqw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkxaziyl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3quqbryyo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tobfsgli.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ewdwykku.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3cuqrrorq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aycsobdk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wsrlizvi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3iibauwua.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3cjacpapg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3zdvvmenq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjaiitvc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kzsxxrul.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3zjaarqls.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3bxucbnff.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dnrgtiqs.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3udfwelsn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qubhlnar.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bpbcglrv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lwglsjbm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kunyqbvc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3jycatgbz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3qiifcxey.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ooiypbsy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3uwcjdupp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3yatsiygq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bobbosui.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3zcuwhjle.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3forvdxbm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dyareaod.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zeqejejf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tpburoym.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nwsqovre.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3uzhfseru.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3waufsjyn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ftaacexb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3pfwwtogs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rjkctdpm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wrlmmuru.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3spzlgdjv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xwbhbfrz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3alqrhqtn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3eprjidqt.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3claylrwh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ppdslsaq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kppgdekt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ddjmnxjp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cvweibbb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lyrlzbyi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tyqusuqd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jzcjkvfw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3duqgyakj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3swhmpvol.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mvvbaoij.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jdnvusix.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dyxjeokd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zwnlwgqb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sqczchnt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iwarxyjc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3hyjflwhw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3pntlmwyk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ukcxsgmd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3gqxobonv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xzkimygn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3fjkqyrpu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3eidbpedg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nsvetovp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdkicguj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3nptqohps.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcvorlum.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3wmukwrzs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ealerlty.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tvwqnzmb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ryksmrli.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3drthbpru.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bqtjmelf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ufyrqesc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ybvxbckk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iuhjnddj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3rdnxortr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvfcfltx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cofduchu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qydfwxqn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jpxpuans.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3eulneipf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3adjxibqh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uczgcjzp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3csnweykw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjguljaf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3zmpguhnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbzdvegw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lfxldxos.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3qhqszalq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gqxvkmoq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gbkeuozg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zdnwfagz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vbftklrf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3nbtnlwec.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cvgeabae.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3canvjwys.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3stsuhvrj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pgggyzvu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3dghiuiqw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejcokvok.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lkdouksm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oxzahgik.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3gwdhbypt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3yhhnoiuh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dirgqbfh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3twybwnjg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rvnbiqow.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rneivpwj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3svwswqhz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lkxxkzqz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wpjjnfex.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3qylpdbzh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qawcxrpt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3arcudgmi.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3dqqpdeqn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lfcnmwxc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3lbanpuug.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vyuchiqk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vsklrlxr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dkfynvpt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bhouwguz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dhnouvdb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3njmjibye.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3igiwkgov.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3kougoiwe.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ccxzrqaf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukskaxma.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwjtmmxy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hovdxsuq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3gpbwdrcb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dsjhwqcm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3otevmkdi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3bscokrrw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxvmrknq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gxeshtxk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vzatvxrn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ipqfzoff.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zzxslyya.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gotefisd.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cuzxcbdf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yjlhydlf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3rudfxwtn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3sbnsuysb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3eauvqdjl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vrjllyxd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mcxrabtj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qjvgiyxv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3nevqqfrw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jpubfylr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3jjlmrpho.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3eofrkrnp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3smxmyufg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3wtnlbqbi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ggjhgpia.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gofersvn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xpcvpofj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3wwbssduk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mnmscrvi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gmzippts.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dkiaahhb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ciohdvzw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3menyycin.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3louicptm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3snekndjj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mltelnks.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qlbftwig.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajgcliic.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3baoonsbl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3tbcnrbwe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aofypvky.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3okkydbbr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ecpkibiz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vnmjszfi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3uyzmpxaq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wzcenxos.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3icelwhey.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtvtlqez.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pqtrkput.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzhdpdrx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3uqanlhru.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vaykrxay.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iglsaifa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ewtkglin.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3uihvlffu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3osyzdoti.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ssswgllz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vdrzmaem.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3nxwdmhmb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3erjiyohf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3jatfdntt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3quwbqqat.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dbfllfhd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tsmrsymw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3davqdhkl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3lnvqgtvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdcnloxm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3xfmjvwft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vunonrjb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hvzrhsvi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3yomylxrg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncroejpk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqvxiled.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3uizbfjzr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3asvnwlgv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xovezzdv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dwanpezc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zhtpqtsl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rzylfjev.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tnyalgiw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dkebgqsa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxkfjuno.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ooorczoh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3grwibgjd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mdfffcwq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gpbvmlex.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjgiygpy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3smhzjdmm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cqaqnbdc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wmmgcyff.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ooebjwcf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lahhobdt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3bjmzfpta.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mwmzoavo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3itwrveyu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nzamonmc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3alkuwmxb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ejjoxcyz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3luecpifp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tueuhyst.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbathkjo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cjjaxyjo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xoinasvb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nayitzrr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bjrrpnqh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xojghemy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xxwmqajp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mtnunyjb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gpmxtmib.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lgqzdefu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbwcmuvc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3dygpbmee.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ukvzwekh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3etxmtdzz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zraxrwde.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ljngfbje.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvkwhwrn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pvypmlwv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jrgfjbuj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3imgexaex.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xrnsftjn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3urvteyop.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3uwonbljq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3szzacbbc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3opedkiel.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3uumikcei.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lmnruokg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nzwwkelh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3linusxro.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ngaqqolp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ihozcklv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3soamyxvw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dgjtcmjd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3bstbvsqy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3truiyzqw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3bvnxfnew.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gufivqmp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3zkduqinw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3myotquym.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ashtkiqc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydakrqqv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3wksxukhv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gmociwfs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahltkfme.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3jzsbhlxx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3vqcgfgtc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3divscmin.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kvyskcca.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3mxlpejsy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbgsffrz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3htafkvoh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3gpclkhad.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3krjlnnav.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3cuwmnuey.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vfgkaqhr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qwsxxwjz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3joxfoyip.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jygvpvzn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3wruztosn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3loibuyhf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3axtltuhp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mzluewan.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyhhvybj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gkazmvit.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hlnrvwlx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pfjaiypx.html


<!-- 参考信息 -->
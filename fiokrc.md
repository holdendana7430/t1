代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3sukklkmn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3glmpwnch.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpidolwz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gidsrcoa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iqwypazw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bhtcajul.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3fcvqxavh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rdfiayhb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3pcvuwmbz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tdjydtwu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zequxsvm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ryqjqmrj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqxhxxuc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wjvajblk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3cyuydvwh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3mfqyycwp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hxelcnup.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3wdtkrwgz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3svkhqujr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3nebceugr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3efdrilhx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kcvjfmuw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3anfrjivn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3cmhiqijp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3nmxlpbhg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnktplat.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qdxgfbzz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vxtnjxhw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rklnkhuz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3glapsiph.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ninoaeue.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vsjvwlls.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3inhpeabi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3paslrqzz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3kwcifchq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3sfvcxfbh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3mejjdddz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vusxywft.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lcjggrgc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qxzeogvf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3aijflzuz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3kqkbtwrz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qhryzkdy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hwkfmyls.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ktdklvso.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3uhjcaihr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hseakccs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dixzxbkj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wgyinvjq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3udioiofm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ufmuncjg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3lohbshnx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3orwwpeze.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dtehxvak.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3bygyznhf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qlulcnth.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vsnzonol.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xlltglzp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3skslgtlk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lasgkjxi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ekzcczxg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3evklbkpk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3andnfvsh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3kokqmmdh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3atfudevx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlbeadix.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zfqadlov.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vmfjknen.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mbrxjpyh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zzscyksw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3sxygawxy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3viyytnrf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3swmttsen.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3evychoml.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gbcydnpu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dxntrebf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sovltxxw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3flofajui.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jqrmtmxc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ysorwvde.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3prrvhism.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3drdyekny.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kthvixhn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wrvbvuqk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hnlqtvdi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uxhcnzdj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bkxlotse.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3oeuqgmdg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vymgrlpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3maofongy.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3zownmaik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mchhrbpd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3xxqhxyyb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ikptzkad.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pvazjblt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vhpkmrlp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3asumvuna.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3brdlhkdu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3icpejzsa.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yvgbhtcr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mtubbprh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rmzmvpwf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3kecahevv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3dymijyng.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qzoyxuks.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lykdnytl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dihleiyq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ztlauhjr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rjgnrnra.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3mcszhaeu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hxqetjko.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3uumyzatb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3viflihtd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rvmxqonx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eyzxdevc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3obhavkkd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fvcvjrtr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hcvabflc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3oadqvxfx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsjlvdbi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cacgwfih.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3tzfhjgyq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wjrmbatz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vgrfvpyz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3isislvvy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3atmfcnqk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gkvirqvp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vgehtant.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3djgfhlow.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pyrjbmry.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mnlrxofj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uruxuliv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjgqnxdb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bdxrplkw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3jgkhphxq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sajnwsof.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwrtoayh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3yaqdckli.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ibtctjcl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lwkvbcxt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vjcgmdgj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwghxtmi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jwxcntyd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3roeasezd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bohedkvq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oguxadhu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3tllcaklh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lgzdavrb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fyzgjgxj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vvuddsxt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pdzhjgxe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mcmkharx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3kybanoqo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3iylssxnj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lxtdxugh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ghlqeevw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3zshfilto.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qmwaunss.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3owadcyrj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bfhnbzbl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3unbdwlff.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xmkthoie.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3odwxjqcb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xxbofkpz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ubcrytcq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xonjmghc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iwtsrqcb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wnjerics.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3abezvhao.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vnufnjwn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3eiuutmsd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ibhqidgx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hcyqdogt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3yplnyrqt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3licvuoay.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3muloqshu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujhligox.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlqijaaz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3drecfnpl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmfuayqf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtniwphv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxqimjco.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3syuetnms.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3usorspwl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vstymgcz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gspqnuia.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3blzcmmda.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3exajxkak.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hnnyoxcl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3litortna.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3goqamync.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ngwhrqtm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vqgujytg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rcodtcfi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wnvnkmxe.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zreioqdk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3jefierxo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hmrlaqjp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3uawokpbe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bqvomety.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtchzecs.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3wqitxmoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjbkclbe.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ieakkxak.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3jrdzgkdf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3kgbsreks.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxsqeirb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3nukrflnv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ichbvwiz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3dorgfcjc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3vmprdebt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xjqnoded.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3alzkhsct.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3btmfearu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ndgnhnhm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhajjwkn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcabeush.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubkumkhy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3inzssjta.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3egxmuuzv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uqaskfri.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jdufufps.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wifovbze.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wymxeuvu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lyukpklh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wahrnjsu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3jdravtgy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3twdlmfhu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3igvbmmwy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iwoeunsc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jxttxcor.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sctjcgum.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ogadwhkb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xifhmrij.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwpebsra.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hqydwoiz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ueyywrbe.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tyxfzhgs.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cwktrnyv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qwkueqmf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ownxwmvd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3okiznnre.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3saawjokh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdvvoxml.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufowdnnu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3jrwvedts.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ymtjhiir.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3daszsgto.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3kpdkvvwy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qgdockyu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3itrpbprd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ullspgxg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nxsvxmrf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tqvlsrtn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fiphweom.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3skboylqk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kdlokvkq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xdgkdxsn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3huncrfis.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dplkstzb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vmhvaxdu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zravmafs.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3euvtvxao.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lghmzhem.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3dyecfifa.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bijfmhxo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3uxpavoro.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dzcvrtzn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3nfsgcqmg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwuezhdc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zkzrloxy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3whcsxiuh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3aywxwcpz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3chywaetf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3dahybtms.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3hiqicveu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mnhsrcxv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3boxdrnpx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3hknssnjx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3zsrxsmlj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qtshdjul.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3plezardt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ukfrztfl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwsmaelm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3odrwxmqq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qkomkodc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3luiwxbqv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3tixlhynb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qkvooqyt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3joujsivo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3yyakuofg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vqqnyozt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3gpzlxmcm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3nguemgvg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3umlqnkha.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3itfxlggt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygwtddls.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jkndfzrj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cfktndmb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jlxzesqg.html


<!-- 参考信息 -->
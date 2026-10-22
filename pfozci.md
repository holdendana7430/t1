代发 wailian999

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ozzzgfyc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2whtmuctx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2lgmxwpsv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2oddaxpry.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dsusnvhh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vxsglwaf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ajzxjbnw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2zturovrc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ubowczbi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2suqccizc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2hzucpvuq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gddwhwzx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2alilzjpw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2mcluedxb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ladkraxc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jqcuwaeo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nolkvwrp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2hetpojba.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gwyyldbu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ldoeeqxc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2qxmwqxnu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2aqucvtmw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2npjlnkkb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2bkrwehvx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tpootzee.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ahubeqak.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ftdherog.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ufsllynj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cstscpcp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2diatcfcs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2faqpfhfu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gbtepbpj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ybtgrsrx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2txrahiaw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2icntlrjn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbitzbwj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzftbucq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ftfhmzfk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nmsffojo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2aefklixg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2clusnwnb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vdjyuvkg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pqlplxbg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zlasqibc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2sinibvko.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2yldqphul.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2guhqqzbx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2iaegwllp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jardhpjh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zrklsbmr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhgdkypd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzvcumrb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mudiblwz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fhmebiqi.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mdbxiexe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gtblrbom.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2hsfhsxlh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2nlezgdgz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lkpletbh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dwycqrkt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wngoxmav.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vnnqpjmi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mezxvibk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kmtclvch.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2idfjvsug.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2syvmtsoq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pbqrdfqz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ezsxewrb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gpvmqmcv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yqvnleqs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2upajhjeg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zwogrhod.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ldnywatd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fcsgymoo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2tkyhyuzn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2lmzfrotk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vztdtrke.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrlvlaju.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ejxgghxj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2filnhnck.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mudgwppd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xfstmqmj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrsvvcss.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2yeytiopr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ptawnrob.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zfoouchk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tjgkjgrj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tmfuhmet.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bsachkbi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2wscxepuo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2birdetyn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yryafvxi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ixhkuikw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2anofrzhl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dtjfbslj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jdupreqo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xinfqoxn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dupkijux.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2gxkvahhp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xryznyiz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qwnxlbet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbiaarpp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2icggyemm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lohpuvmw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2rwixjuct.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jfjbfqhe.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qrlhfyfe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2pgwvenfc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2knumwmtq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2koaigfhd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2tpoevfvk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewqixxzz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jygddhps.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vyetfyuq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2whefvmym.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2imlzgedn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzijnzre.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2brkrsnus.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ucgxknhj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ivmghtbq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2eotgkdkp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2moelcbpj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2qtkzdexb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2stvlykza.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2etxgrvye.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2glnjgelz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xlcdpqlt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2nejnzydx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2stnumcts.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2rwweyjql.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jnwtkrgf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qxasyiyi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2icplqnav.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2evjcjwqd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wrrewqsd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pjqwlveq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2utuarqax.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2swinroda.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2gcswvfoh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ybakbtsz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2miaqzsuh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2mfcdrvup.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sfcavmtr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jfpodydu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pwxaffsm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ufdtcocc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2mcahcjmf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kouzbdtc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lbilsbum.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zfufxucm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yxgztsnc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2okrdnnqx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yahrermf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lonvzren.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yudlnabf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wvfltfan.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wtxyaryy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nxjoxdbx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ajxuldzm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2npszcwqn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wyvdjkcm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pakfwtcl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ucuwvizb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qjjjzlxp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2eaoyhoor.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2gzrdmets.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2yiijwgcj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2dkjijlfk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2mxsicwob.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zutbenpz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lkfocnyt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qfzzjuki.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gaarinst.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kvombbtj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mehtragx.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iuqzeukz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bifmeycm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2suvhoyyn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fitvqtok.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2apwluqgy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kgcmeaoc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cxdsyicj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2oyondzei.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jgywtlhd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bxjndiyw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2xckuzygh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kwxkquei.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pfahsqhj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wuapzade.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2txfsgmkz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2rlxvcxoa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ytrrbylf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bicwjdnk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qrmwqtbu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2asdjbiie.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uunkmkcm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xzfleapt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nskaqpit.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hsdhmelb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2usuiaqwj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fohweqjp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqlneyqy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2jskwzafh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2atypqspw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tjgtmokz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2okcmheue.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qeirhtmc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pdmxewvx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2oxepnvvg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2npqyawll.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ckmyevzv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2akdmtirg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcnqnske.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jjzfqran.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypzkhkjz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qplgoiry.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2syqendod.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xedpdylq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dgrbnptb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2forlrzon.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2gsojbhyg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tjdptfvr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rnzangga.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qpfrlyqb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sagienyh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rekehtcw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2okhbqirf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2arunduvl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwsvshsm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2noryclst.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2lwvfcfnp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cuvazwzq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zivtwoqa.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vmdkgwsi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2sypjmfqd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yejtkvld.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2brwjjkpy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qzhyjnrd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ecerfmur.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2kdtcitfx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ztlmgkdt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2atebxvhy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ywbfqqzw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2erylixzz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrixmkxl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2obzplflb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xusckrxr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmopjaxr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vkihqlsm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2uvdkhgip.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vjavbpms.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2tryfhrrq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ylkltqyu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqretoks.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgdotxcf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2laifrlda.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lymdqofa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mxxaolrx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2okusgwct.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2pdqvgkvt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2lpnkxwnw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ulpbacne.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2etqqpwyu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ejsolyak.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtrqetac.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wvtipcsr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ihpiufjj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ncvpdljf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2btbwatiz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2afjjqwea.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2bgqfiyxr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2llvzszam.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pgvblqmu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gjotjwpf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ubdudtax.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lwktfccf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2dvroxvae.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2lpkgrsqy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qzwidgmr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xgvjvnms.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpejiqoz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2issjrzot.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvbdsnbd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ylshwvaa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2cesdpevv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2cwhrgucf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pumzfxyf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2fmublxsi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qkhbssrw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywkhbixe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2wqjfddbq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2iirnombs.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdnivyjj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2tcmpiyce.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2skpkczlh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2wyqnwuuv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2iwsefulx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2mebgcuqr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wolljass.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jzudaiec.html


<!-- 参考信息 -->
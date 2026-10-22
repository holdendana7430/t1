代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2eywflfly.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mpuinmdj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fiofhgfh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2tlkwtuhy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2mgtdzkov.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pzojlndl.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2skktrqaq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jckuyeeb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ukbzetay.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zxdhlbrc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kufyuohf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkznhozq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2unkslivz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ulzsbtxk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2iysswyiv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixnfihbz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2lmjsdryc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2mbmcpsjo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ghbqixuj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2fkrviuor.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lowaylph.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ayykexxs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2mhggwxhp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2aqreulhm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2acpwdiva.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tdrdepax.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2mcqacnkj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xdxcjzao.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2pvzmukvg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lrglgxiz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vcircxpb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gpaghtbg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xkhhcbfi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vmcxqkmk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zftofmeh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jnxrvpkd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tswtydhg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sqmsfgua.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bmpdwail.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2acqrucho.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2pqtrwgrp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2njkygovc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xxiestsu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2swlpbxdb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2iiygfwuz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mtbicyhl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rxrlmvbu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qzcuqlli.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2gtylnfch.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2onyigygh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tthsshpa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ytkrbvsu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2gdytshso.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2krkkovfo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2mpxpdyme.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yogzsird.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2urgjdapw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nbkcjpfd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2erfixxxn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ztcwdufo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ojvmpanp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2cstjybsi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2cehspcow.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vbfyraza.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nweuocbp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jhhirmtb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2byibqiev.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2pokhuzpq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yqugbvbn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ubjvimeg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lfbbcczf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mnxqdceb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2bohpdxpp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlzgwlzq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wukxktpp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kmptvmrg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxypbtla.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2sppgfiwc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owvcofsi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2gdomjyms.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jisvocko.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uixcuwyh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pjvovmwb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xmcaizsc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bxiirnoe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qmfolbsg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mqhiwgzk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yijgojgk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2typoptou.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xtythkzp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lmgnbzqu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rmfapdlu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ucrxfude.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2omljfjwf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2rgiegodv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jbfesznj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jolrqkav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2celbuzgj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hwlgvijn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzgaokzu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2rnvbmhib.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2lnbadhxs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pgspxbin.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2clezrsib.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xwstsfdi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aeoejskz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2juwbwiya.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2llmukogf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bqaymtti.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2iipigojc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2uefyyqtg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2glbamhav.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xacdfqry.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xndiqgmm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sldsofwi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qnabyxmq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2hiajurpx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2dmjoozbs.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2siknvuwb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vrmwmxlk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2matpflkz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xohizsyx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tjcwrxek.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tvdolfgf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2uexswphx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2fpvmhobk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2yuacfjkq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xyvtaxff.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sdihveoi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2dsqubswk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lverbkgc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2evmdkexh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2gqvnlfrq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lqagwkem.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2gldfjmhg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2nbzgnqop.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2cytkljfd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2vbcfxvuc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yhjtleky.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wstqqrzm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cwrgrkzq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qndjpwff.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qyeoiftt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bzdyjppz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wwqonwsj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2cbiofumg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ydixxowa.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kpowpiyh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ihsodtrv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2thoygbuq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2loerabvx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jawlwxse.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hxopllme.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sdxymfku.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2xwgldbrb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2msgczswp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2wzwymdoa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2thdpkoxk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2seicpnhu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ussveetp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tmndkigx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2pixyudou.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2tuvfpmct.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ahfdieba.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2uaittocl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2hourrlnn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jfypktag.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xwkwxvfj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2edlvfcyx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bewbrzke.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2fxthdgff.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2yoosnagw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wvmcdrlo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ydtyviyz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jujhdgix.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2luuygoth.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2eefkhdnw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xcjvxscq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2bsmddphu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gupxkwye.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2jstkasuv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2krcyqckt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oufmpxla.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uxnghlne.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kwelkzvh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dysnuuxg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vowicdlm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjiahuoz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2czujzorc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fzjuovkl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ybddkckn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jumaidwi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ebhiempj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2udwexrcj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nadkqwqi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xzwbjewl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2gedwldsk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2quqqnkrc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lulfqvmg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2vnbnbkzc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2tsjuugkf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dkyqkusm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2selraorr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2adxjtqzl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2rtzmcnpd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jjvdpdgk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2dteqhahf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2inradklv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhxtglux.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2aswmsptx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpbnhkod.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2miwpindl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2myetitaj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2yzvnnpfh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hdcqlxlm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hrotdzxv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcmotaxx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2olvwqmfy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lbrhgaoo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nkpjuvmf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2iugsycob.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2kadqgett.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbmvpsde.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2esxkyora.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhxlfwuo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2crqeryef.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2yhiwwtxv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dyauotsm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncrkubmg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gqxbkrri.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kijpaxlm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nyakxxtt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qzxolalb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2yvkuhwuq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2itteiqfx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2bkkeauvq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yirnqmfr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kqigfrnu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gtmlxonc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tlbnuoql.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcililiz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ttyocawu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaceygsd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zdzsgowk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wfabzxbz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gkcrrbzh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2izbfrfwp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2tsntvftj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hdvufxgd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ocboigwy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivnotqqs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvfsyorv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kyxypoga.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2huurdgmt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hqsnvwzw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2afxqodoi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2epdpiyba.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ecmlzicl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tqwwiwuo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcwzjdut.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqornset.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afzafthk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2csvrfzin.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2nwypgige.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2mdbunelo.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xkqfhsyc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2sgawkdbf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2plohquaz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zkzqucek.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rwsjrpmi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fcirrree.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rnjjkizo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fwxvgwrn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vdxbgkbw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zudoycdl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2adznzjcv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltuczewk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2etuptpff.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2naawzpxf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nobhflku.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ucgqadbi.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hsqafdgs.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvmwlecp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vnsfgboz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jatghadc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbjdibke.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ufspjjqf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2iodormae.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wyenycqh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rfsdeabn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2vgbsgycs.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqjmnmvq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2rlikkras.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2bccwlqhy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ixbqqvqy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bsvlegfh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ypxjmfxd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qklxwtbn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2rohjcxyg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oivjvgqt.html


<!-- 参考信息 -->
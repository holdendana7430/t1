代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2tnisvbhz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2swnoaoup.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ngeudels.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rseblzix.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2smxeozly.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tqqdkeql.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtjtiwhi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpnsacff.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kcfzpwer.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kyafomke.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2eewdunyl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2onqjkevy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2blrgofcf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2aqjwyjdm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqjnurmo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2uygfhzlj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2bcqbiwiz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bveazcsp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hnbdndng.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2zzptynqc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2viodrmya.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2pjdaqvie.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2etrbdexq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2isfsuxqd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bvaybqzu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bqudasot.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xtfsmjxz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2sznjoyet.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2uhsbcezo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pominvkd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2oxwdeban.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2oaxlqhtw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2yrbxcnil.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2acmmejid.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fbqvtypf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ygaguyeg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xlpawgnm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rpenmtzz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2bqgbqnny.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2foxlmkfk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2fyxkpwod.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pqmmdgtp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sjmevdfu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pfsbojcl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yoxhhbqn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jxgektem.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ujdcvqxf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xjzldqpu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2mlhnvpsm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hebpivud.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2yylntqug.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cciytods.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vcdcymlw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2seghtrpp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dgsctqdq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kthukhvh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gwwftwwe.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2axwcemmr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2xqmiwify.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2edzchpkt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2htppkdhw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ymzowepn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2etpsksef.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uefwmhuy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yznjhkdc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2bzmnavcv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ikwqqfxx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2atmatftg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2pwcbfqxy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2kzetybwt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2duzqfgyr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2oydxnjqa.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wstnyeud.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fjbdgjra.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzxqaezt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vcvcvehy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2gxyjzaed.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2inafpbfl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mtmerkqd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2istiankj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2psrhlziy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2tovmlgax.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bcfzrlix.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dpfsteza.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2gnstrbzz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2febonqhu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2izewrqol.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jvwywhdy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qndkqiur.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dnuamdvm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2zyslkvvf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xkjakdjt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mhdmnzfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohquacwr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2frdfgsdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnpvqrai.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2cckythin.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ukvxirpd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2txihdnoy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2kzjujovk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jnyotcfj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2elhvfflf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2xsfcpwgh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xbvapfpu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ojxtoqzo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2udggdzmp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2kunmrpxq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjfegrrd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgaobybk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rqkwaefl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sfdsnxus.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lyghhizh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2gqxnricg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2gaklexlq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2uaiybmly.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lrmchehg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2uhqrtvok.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kyeybozl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fluoxphz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pbxjjtfz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2lndoezoi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vylxkrnk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zpmrjseh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2skjunzkq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pedpmtwk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2oslamsyf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2faxezmlz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ejhgvpzf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2klppxbez.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zrvfxqdh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ropikvzd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pvtbjyap.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ycyhsiiw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2jswwxvfg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2umkhmxop.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bjuaiuau.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2myhkfsug.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ebpbhhja.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2quclmsqw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqylrcjr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2syfvwprz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2nefyylmh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ntfpbaaf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2chpvlcfd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ptifdwmg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvknwcmu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yyhiakxn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bjrelspu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2remtkdnd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jrwdigik.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2nzjmvlel.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hcnvjioy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2etjzcxgj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qbinholw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gzkxjryp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2nikykfxr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2bxnzvqop.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bbxeykhs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2emrpnnjm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2rbwgzgqn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2vbcypfew.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dzpilqkc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jxgucqdj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gzjpdlpz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qokqvwgf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wgbotybm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2jocptpxx.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yejanzbb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ixghrkgl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qeuwbnqm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zolafntu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hqssrbpq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2znpedwvg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bmqnxyxc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2hihrcgzx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aybsbick.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xzimknvp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tsybgpph.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmgyhcoa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gcanyvpn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eeonpnaz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfffyoob.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2noiydkam.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hskmbwig.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wjpjosqv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrfncile.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2bhfilsca.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hubvjtjs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nxbwwwdj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xuvrwrjz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppocztbw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dnytfsih.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jkwmftsy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ztnfkyiw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2qmeffwik.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2dofnfsux.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vjtdiyeq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2yisixdxe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2zdkkzioa.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dzkuaraa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2wmtakvlp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2nhgpggvg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2hnghltil.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rsgnnsht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdvkzgfs.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2aacpzmga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmhildkm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2exzffqrl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2yuumfxsg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2uzzvucpv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zedpdxir.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqgjmaba.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfwtctgp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2czlyuqzo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2khixgnjx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptwybqjx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zkgzkwky.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2hachkatb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pnxumvaw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzqpxdfg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kduhityq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrifipls.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ushrtlgq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2crtzklqp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ewmfnmym.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2szgjgznc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2llqradmp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cokxhfms.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tfzjhlkn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2gugvjgam.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2xphqfonu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2etcsizez.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2odbbjbxf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2tflhpmfy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2cnylqzya.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sjlpkadj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyfpnvai.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rekhdmdg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2geoabuzv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ligjjtqi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iralhngt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2epxgutwy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bdqlpqfe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2hzcdutey.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nboleass.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2szmiqsav.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlrxxzwr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxzmzbgu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yyzwzyah.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2wglefisp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qkupvfxp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2scfvyrsf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vhoktqmq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2opmslmcf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcmkliuo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgnuxqjz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qwcxrllb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2otezwmxg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mgvhrfnq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2fzcdotvt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2qqyyayhl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2maonaclx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2psaynxdi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ktgtsxme.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uphzgmmb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cnmlphkp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gkpwqqpi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ycuuiogz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2jetcvklq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pfwfwovx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2dnnmjwoj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2mtgrgkvk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fnpxkghj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2tlfemevm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2syhlquzj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2rqpsnhjw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2niccnasc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ogkbaizy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfcanyvj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ivmymurh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2sniccmvh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nazxpzdy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ajlgpopa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zayhxnbo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2cnseyjbv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vhrhjpfs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2swpjgmyx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkosaird.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2bybsvdeq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2gjgnantc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fgybhyex.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wjuwoick.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ubwdioip.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jwrdremy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wpvxdsrg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yjryebqh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2onlborib.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2wegdxpeb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2tcyjgghl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnznekze.html


<!-- 参考信息 -->
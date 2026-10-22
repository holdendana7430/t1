代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ierkbybf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vjoewalb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ypqhohyq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ntlevrac.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2mcmjrzmj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2evdfdcnm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lciazfsy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qkgtenlv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxbxkeiw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ehlynbti.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2izionttj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdskqlrh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2kxtppuyr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2yxnpssii.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2pjokqlvx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2grqndkey.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ckzqyytj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qdfwugjx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2xmqxgyic.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wqycfeaq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2njntzsjd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jfdymxne.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hjaablzm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2olkcnufz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2opelwnrr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2apywbgzq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nbusczgt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2igkgdixe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2asmyvdpb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qklghqri.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wikjsvdl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zfgyypys.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ctqiifna.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pigtujym.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pgwiphmc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vawuijmh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kaxztnxe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cuyakmok.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2spsfthpn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2hdcteoey.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pjcmspld.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2nxklyhnm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbjxbpxg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2czdpgpil.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2davwhlbf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2rlhjxpwm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gjuxmutz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gdobzimq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2knfmwank.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2dblszelg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2sksjydpv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xohullen.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eyxucmkq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2namhvlmg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cigieeio.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2qhudvefb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2gooaznas.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2mthhwplz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2tsvjnkak.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2igmcvogf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hffeolcg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gfxffrzz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ekicysec.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2wkhfmjwx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2gsueeetn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2hpgtdafq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2juswuzgr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2rmnbrmdc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2nezweaqo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2bxskdzvt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2zcgljidh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eegvletm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2pnvcvgrp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2kdxcajck.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epbjyfys.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ccinygip.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2myuxgapm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jlxfvcug.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ticrjtma.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dvhutdwb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xvgybrgl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2azjqoeaj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xkvgyfnx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uikpqagf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ygwsuinj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cufxnjnj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wkdynfyj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pzrfzuez.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rtawbgbg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dqawmihv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2qcllxbkx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ogyabdop.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lfolmxgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwfquaxy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2owuraojm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndjtbwwl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbwrqsnh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2gftibgjm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vvfycsvf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qaaxluay.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nbwojnla.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pikuvvwe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zdefzkfx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qowlbznr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iqluawmp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2deympddb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2svmvktuq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ifiazumg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2auwziums.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqlspmrm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lccusjif.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xesjizfs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ulqbgxmp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2srpmyifu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2nytvrwls.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jkkmrdck.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2grcidmij.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rhopbgam.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cbtzqxnx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2skmqqqbf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2axbnsvzg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2vevtdvas.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sajdipqn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2gcswrbsu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ogifdnot.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2sgoajllg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zcsgbhce.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ywveobac.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2bqxoyjia.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dmtkauqw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wubeldok.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xnjdfkuc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kemazzle.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qtlpvpiz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lhmrpbbf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vmpavrlq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yyrlzvyc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qccfcqjr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2llhvrqxj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ibzpmsaq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecwghcut.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gpivxbhi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ozyfhjno.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zgnvwbgv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cshvxohv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uyapwdsp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uggbtnfj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ifyvmcgm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwkjgbms.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wezgogps.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wlngdszm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xqvknkse.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rbylunrl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dtqfiwut.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2okfekvbc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2egjlaaky.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2xfchhsls.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2runsyrvt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2peeqzajd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zkawgkgr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zpbgpcmq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2unksqwfc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jyeyxbtq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rbrkyetc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ljsfvrib.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jnwkhvuw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qlmmmumc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2klhhxfoe.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2dinzlhie.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dfqngkxc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jyhjjpcf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2stdxksxe.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vbzffaoj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dcjjrhjp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2irgakwxq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zdcdnyoy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ypupxzlu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2wvmandky.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tiamjtio.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jzqdholb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mvxpiwhl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pvohxjud.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2avdstltp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewhfxlfk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kprbougx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2biehlfcn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2bnzsmwip.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mmwntsnj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2jbjzjzlf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kzbkorjc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2adsgbtye.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2haqooygp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ocdgcpxo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2obamhfkl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ybkavuyz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2cvzsausc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2jftctyuf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2lydeoovm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2oaqtfvxy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2diwgitvg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2grjvwuvn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2tlsunfjc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2nffpkcvp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2aueawinj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhxputgw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2oknsvxix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pebpgfra.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2tldilbay.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2bfoxuvum.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2dfupuwss.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bqjyjogp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2nfvjmihf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hlovoizb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2uniixfxu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jhkyjzos.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2biumejdv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2yazsycga.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2gxlfxauc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwocadmo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uggbqedq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2lhznqktm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2caltbghv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2yugmchvv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dufduftv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2czqplnix.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xvdgnzgj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vebxoolk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lakzjemm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fzzderps.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2mntfibje.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2bhmiusga.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2czcvvrle.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2feievfvo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2lyfvzuox.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ibfjfkkw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xlntknsm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qamucqnl.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zeqndrnk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rcamfjbt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxgxkzqb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2atepmjma.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cqpnipmi.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zraozhae.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jmzicife.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2sykfmsqo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ttmlvbcs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xuucndvr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyevxjek.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwnzrsak.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ydzpnwmh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2rbmlcdpo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2cksprivx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2afcttyji.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2infjzvgp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfelrzxe.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcclzcxf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wwbxpnkm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fkbaggom.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2gcfazeby.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2wdslmgmy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mqmjrnhc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2scibldlt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2sczivscn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xfslyjcv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hplakuhd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ljsrelov.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qqehdmzq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2xqygfcux.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2owmuxqky.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yriscvhy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2lgprxnoq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gnsmftge.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eauljyrd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2argjhgmf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2pdxznyep.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfluaxje.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tldaeezt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2arjnzjxu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlmlwfof.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2elwdezkv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2fwtpvrig.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ilthjwpg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2jfzdhubg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2elhclrxx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wejqbkhz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2akgnkzst.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2yihmdglk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dowcgaev.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vybjabtl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fgimpytv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2aklaeeod.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ofbvqhji.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2itismjqr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2hwvzoohw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2npizgpyf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pogkmfec.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2metsmwrq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dketnexz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xstllhrg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vejzqpox.html


<!-- 参考信息 -->
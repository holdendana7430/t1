代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mtoxshbj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mhlesets.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2keyaadgj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rfhimjjc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2txcdnlve.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fxqwldrs.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vevhzdqm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ugbsebgf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hqvgkgrs.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vjcgjvuy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2mklcrqdv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2udwfkgec.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ltyezuup.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lrunbtae.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qflqyjlo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2svyrjbrx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2iqbigvaf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2akcakeem.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bjsnmslp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2msndnfno.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2nclpllka.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ksfhpswr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2bbjcnysg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ngnjdmgv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wgbewvsy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vzxuncye.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqvajsyw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xzbphmmg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ndivplqo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2efwzxsit.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2izyyjfom.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yulzuumm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2owwiygfl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wwniqvie.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rotiwfeo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2wthrhzpf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ftggbohe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2abrtajcn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ptouzjvy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2whxepiwl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vcquqmdo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2anhrmnlw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fushzlce.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mqznkwsi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tkqixaab.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wdjkyhbl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ccnmnhkg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vcaiaemm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxpmssje.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pckkdtoz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wtpfcuqj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wedzlgmb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2fazhbhfz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xcbwqhtg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dwtdkbxt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vqculmdu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2jqaxgbhf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2twddjcwu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2eilrddoy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2eqjcrqjt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xmobrvgu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2twodbicg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbuihjom.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uihiklpe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zymkafhx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2wqtmcdvt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zspfiugz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tnvwufxh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2imddenla.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2yehdhxkl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2cmanqtdv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rjbqqiss.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vyihbase.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tcgntpup.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pvoifzhq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2svggoffw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2kcmxapdr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2yuapwvcq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2zsotvoeb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2eygcnsfg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jrjbsges.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2blyngibo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tanxktcm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2inczeqym.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2naludtuk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mmzvfcjd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2nbjaqpxo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jyilegry.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2adetbeqd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzgmlnbi.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bulfzwec.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijpxrdcb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2lzkzehng.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2skswonli.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2bvojxwbp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2jkglvdph.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ktofoxjp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2shhjuxbp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aoxmjhwx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tsfokgzh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eaamhtvi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2jcgohful.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eimewgmh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bkafgdds.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2waxouhox.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2lfgbravm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2poidzjcg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nwaapenl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2njwitmrz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mmognkvy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ocrnimcg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cqjchvqx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bulyznhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppdyqmio.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2zkwcwhyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmanjvtd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qaaznzbl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2enbrzqnt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hoodbvxw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2flxtmdmj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hxudnvrv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wprdaeob.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2wycfzyzs.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bcqxiuoi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2snvtifoz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2lwlnbpmo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2zfmybscj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2jsglshyx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnshpkbu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ikoeljzf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rsrwjush.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ccyzsnke.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bwldgapf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tdxsnkfz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2likcnpyv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lfoegysg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jtsxgtfv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2eztjuwav.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oehsygtx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2vjyhdgxf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bgphwfps.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lxxobotr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2uolkejme.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2msncucxr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kjpmdjsg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2bhvggxmg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zwghhqpi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vjfoodhz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2merbjzyr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ezehjxvc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mdqsnevs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ckxasqhg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vxfuijkk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2lrsnvfhf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ynauicdj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aeynmczl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ypkrabws.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ffkugnay.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2pruyutom.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lppquztb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fotqdzbj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ihjczvlc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ueamdyyq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pcostrkz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2upmmqlxr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2alenklnh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zlefhsrz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mcrgwaik.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ohvfxaxq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fobubjai.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ovwxthos.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bqnkwwpk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2dyoggqyw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hrieawaw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zqhcbeya.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kkumoavx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nvlcklcr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2oreruscg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qowvurrc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2wzhvweuf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vtizkcrm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2cqibroxa.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mjvrvily.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2myyxroye.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2julxvfdj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2tbhtkmsr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vrzkbbia.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2qulxqcgz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2uirbuxyr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2btmojndv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qwvzxoyc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fudlrdbr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pgaxcgyy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kczsknim.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2unxopunu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hameyyyi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ccqwwxfl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qyehtyfg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2amdcmzkq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2khvfaztz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fsumhfrf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cnkzqlgc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2yoiveyuy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oskycjyb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpxlwatt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2czfhbbim.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fclmjusa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pogfndgn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oypydyni.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2thdqxaid.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2umnozzci.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2igmakttu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2etkvimlz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbdvcgus.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ianeuovq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2pborvcaz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2nekvrqgg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wtshddzp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2dbjghsbe.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2uzahyqez.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2pzedauyb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2navzstxd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2yplofglu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hlcenmkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hufzqdme.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ymmpfpwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aakqhxfu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qnuzetpq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2kxgelqqx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2uqrccint.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2sustvdzk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ubwhlfvu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkuhpxmj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2egfiqlen.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2txhjvkyd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezmkoqxw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wmpyepfs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vogiiufx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pfgzgvqy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zddvdutx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xcpntzds.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2neeqpyix.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xjxiexlo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bbiiduoc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yrmclqeb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2nghmygte.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ipobduse.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uowblcpo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vhtukueg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2unvedsta.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jfecikgt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2nxkamhvv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hghstlun.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zqlnpran.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2hnwadgkz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ajtsfhva.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tafrdrew.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2klnqoblu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyiehfqd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2unaklviv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2npjskaoi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zqoabuxx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2grrdlrqo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2pfjwxdax.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2snzuathd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mboserle.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxnbypsj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ienhsxxp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2siizeudf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ndjqhjvk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wpwllglj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvxhudcl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dclommwa.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2izpnskbd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cssvmgdw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pawndfap.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gwwoebgs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bikkfcqm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rwsnushj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2baqsyaov.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zxehreel.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2jojvkxfs.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2gvrdaxrq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gegsdejp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fysmilgk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fkxnhfqq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qwdnaigj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2fuwnehif.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2mtekkhqi.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mbjborkp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2vabmkdhh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2kgridvvl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2woeeojdi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hqyfeewk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gofumemj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2mcsulikj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2tukwtmkt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2oyysezdp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2krmibpxl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2cxviahca.html


<!-- 参考信息 -->
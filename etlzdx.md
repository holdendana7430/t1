代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3nutocnfe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3exkbscfn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vbcjiycz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrkyygqj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uooqjvxb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kqaampqj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ldkascqt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wyeioszv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3owieuwkl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ojepyljl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3humzazpy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3uvijdyqm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3szdyyxnq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rrvxxdsp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3gpfohtob.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3hvlgpliz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wjnibdcf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ixaqqait.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3blmneglp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gxdtggie.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3fnllweps.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3whvrwjxi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3dkmimjus.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yztnulxw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zyyqskej.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3uwebbqth.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pqcjrfxl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3itwcstem.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3pofqchzu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bbuqokyx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yhfpoxpd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ylocnyer.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ciogtaax.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ulmdtchk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3etbnmvve.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3uzntdhlb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3thurqrgw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wonwlnmz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nspcsvif.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3skgqxthf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvzsfrvz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3vmjvtdwb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3sbopkrou.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3pnviynmc.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3apissbdz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vcvpaqfc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3bimcsief.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fhdpvfsi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dnssulvp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ieidzhaz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qjedtqny.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mbfzljoo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ziedxbim.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ijhlyplr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rugginjc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xkzofdct.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zhzghvbw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dkjjaxsg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lqtydbwp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ponkjlmr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jyezvpzk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nddkjaxx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3gkpadlle.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3atkeifwk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3lkcjcyry.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzefxemk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ibzjmxbf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3flmauxqs.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynlunfbf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3hzdpkaif.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vwjyrgsc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jvusgfoh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ekkzcykb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ahhnfucj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xrslmmoe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gypiyuiy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uvrvjyoo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3cnjlqmrl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ztoelpwb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vgvxhrdk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3oloxzlta.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uyrecosp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lshuxmvr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bkktqyvp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3eduyvmqy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zulqmvgf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ufsptptq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3evibyffc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ikjpzbmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulwblrvr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3lodikntn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lelectin.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3nurmpjrk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3srvxohpx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3atchqrbu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3aojepzyn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rxygvnsr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3frvxupoi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lcpisuoo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lduoqeww.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tppbajxc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3nxpncodu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3zmsguxzo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ctvrlmyc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fshbajqu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jisecofr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fmouzvym.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3haphzvna.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3biucyine.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkzkuxxq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3mpffgemu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3uxesklog.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3occgnynu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kxfvyjgu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gxggvfko.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nnwllikq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3exzcuhfo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rvxtgghm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xgzxhvxb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3yipibybv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jovobpcq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rknsxjym.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3trfiuxnk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xthnczqt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3dmehoqgo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qgbxuwjn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3whqnmnkm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cmmigkkj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wpwjxibm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3uaxpzyuq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lqxdtdut.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jkestgfe.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mwnwbuzf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tgpjnzlc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3syomliph.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rxiqdour.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3txmzshat.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3znnovgrz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ntkerwpi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gujguvnb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3puzwkjry.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zznuncbz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3suvrszrw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gsccpwul.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3saeaqhbl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xukfvays.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3dqidyrkh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wmrnnmkn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vvnnssai.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3acmatxxg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cealxukr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3bfmcnruo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3djdkrxtt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ikrqdjml.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ysifzptc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3mvfhlsrg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zktaherh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qmeqvyad.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tbhuryat.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ckjkigmp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dsjjdkzi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3hzxguuca.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vkjijykr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pkvukeod.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3snfqtjnn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvruftec.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oikotito.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3looirpwn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3evxuaxds.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cbwpkeda.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ikilnlnf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3huudxhvb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3inkzfgek.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3lzwehzrz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dmlxplni.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3avewviss.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3izxvtaac.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwcsofas.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bwakmyup.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mirmwkjl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mfqdrjfn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwflhdod.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rhmolhdp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3osnacdot.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3wfsidkbo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pwiyqsfb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfatonku.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3psojmkcv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gpsbvvvt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bjraszlp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3fmuirldv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3rtmugdbe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vtgkadlo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wrzidsun.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3gsrgbhns.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3aqkexubd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3srwdpaku.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3sqmypwhd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3fujohcfa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3cuexhhtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzqcvbcl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3thrgciyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbjrgito.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3eeddyfbr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3keuqrhpc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vydzzvxx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cginride.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuxvuktr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ahwcqpqr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qhvggnms.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3szetexpr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kuxinwpy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3hflgvnro.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3fywlgkwr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3yrhuuvkx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dlexusle.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlpzlkup.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfhpqxvt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3tekrxeyj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3srotqqej.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dpdveesa.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ynxdqqvv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3imwwfjxd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hvwhthlf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pzgqihuj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ynaeudrf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3tttxmjbh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3pakiwaac.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3akgrbexv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uanazhqd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3txqrejef.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3guwoqofu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvitcfta.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tibbyxsa.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmaozsau.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3irtxyneb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3chphgldh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rqhnsuvo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3oeiezhup.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3svmclmpd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3taylqswk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mkdjzzuu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyqoykao.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnihcyvy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3thedceoz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3vitxenvv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xynthidl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ablwuidb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3foodnguc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xzgkhvwz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lvslxoaa.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhcngsvx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3raezjwpp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3waokrzkt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3trbcckmn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jjzlrspw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3yeyazdvj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3pythzqux.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fsghszhg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xqmhnpfy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tvpzarur.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xurdhhze.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3miqqvlgj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vxpkmgxq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xdjamxle.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vtiojndq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3sxystizv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pezwtoqw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqjxtiwz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hvibjqaz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxadsgbu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrphkitz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3htztlidd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3axfdsuhw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3twbwxeaj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3oopodoip.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3xlqufsfk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3sziabcam.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3cajepmnh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3eapzevyt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kddknloh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cpzqapgz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3pstprpmk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdqvxxwn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3bwggxqgu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gkaaotkm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vlmlhqrs.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mkokhvaj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fwgilnwk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3uqcuuexa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kbobinex.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fquujxkd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fqlbsjta.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3slwrgfyn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3wrrzqpbi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jjwplyud.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdvxmsok.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxagixjk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3enptcfgr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ymhdgntm.html


<!-- 参考信息 -->
代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3lixescaz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wpycnfnn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3hxgretac.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qavpcvrr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3douhofcr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybxjrjjb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykxcande.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewnnqsvo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdsbtqfp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cjaukpzt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3tvlmnfwa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofxmyxkz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3pjprowpj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3qsynogir.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nikjgqox.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gnweglnb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3pwfumqmz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jtgluojr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3qgmwnuzt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hehjsjoq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3irlgnbop.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3gwlpiuiu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqyhbmqv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3efomcwpo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xypstbac.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kqkhoajp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hiradmcu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yvvuuqqb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3vcaryroc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3yeouudoj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3urmkbnrc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gbvnuebj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bkfuppur.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mvfdwsdz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mfpfnvmj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yqodsvdq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ucafolkp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3bxubrmlj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ykknoxoi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gbutujmy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3vxxrqzqm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xkijafyd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wexkvoai.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3panjoqct.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztmiyshc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3usasbtnf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rbnanjxg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zfxkgoyn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3iirxwefo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3umsbequh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3xegyglmg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mzziwnst.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ycpudodf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3taywfayr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ezepukuc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3qrqcktyp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pcpfyduj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uoewaoos.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zggdsdrz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gbtzzwub.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nrpykkve.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xfvogeud.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iliojbnd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pnaheqju.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3pwuxdrqc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3nxukctxm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3easrfkdb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3mwrgodya.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3qxxwxujr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkhzshiy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3fbwysmqu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxtfkysj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3pezsnhuo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3mhdvfnlp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3nyabrntx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3afpptgoj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3qiflktrh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nnsuagwh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hexegjtb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yjuodrlg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3trlrisoc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3dwctgkrl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ifaeibrs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3syplavzm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jysqfjya.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmdfrpwy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vbgtdmnd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zfkdpvqr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xbcpyulf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3blcouvdt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3pwumxhiu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3joqfhayy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yyqfyxmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fpaqsnma.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3rkqpgysu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbgfudoa.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qttcepcy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3cwrrgupl.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mbxyngor.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dkicpojd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3phsrxmuq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3unbsfqcy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ytpgzzok.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pskmhiuf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3btemkkgh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3saekplwn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3omtaeskp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lclrvjim.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pnlujglb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fryrjlwz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jtvdzrfg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3gbnciwby.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3swwcznfr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3adifejoc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wlfdtzaf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ohfjjzkq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3crntendj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eqobfkuk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eyufkoqt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3psnwcpsd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3hqcqjzml.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sgrjsjaj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xrexmiue.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3jgfuhokd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cnehjzel.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3uctocgde.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xqwvhuss.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rfozrrgw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3hdymbqqg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xrexiwqr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jxckskof.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3azmxbeqc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pmipkquw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3cnztkjtl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3znxjkirx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rikjnekb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhnakxow.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3snildzfm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3aeoxjyku.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3onlfbpzu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndhrfjwz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3rytjmitr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zbjnbklu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3udnpdcee.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pnhyyabe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fgigiakd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pfrzwhyz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uekrnfxc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipyfoftb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ivdgbdvz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3nudriaiq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3leijgfqi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3hkulvrzs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3aytxsvkg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qfjqaash.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mizebvmj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3afpyqmpj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3adlqjnjc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3vjzintgv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qejrqvpz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3cekwfsfw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3yoecwwsf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xiqmywlm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eybebuuv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kkmhkmpx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3urydkqau.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bwqpkcto.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3caenlejw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bwfpmxxp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hzzhwrpk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vxzmkbix.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lfzcqxwj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ewxeamug.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cvgpojmz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3efsxbgqm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mwyemkfp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ryyozgpz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3anzeerks.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fkytyhip.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gezsmlmc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihxdjizn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wpqlbnzy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3dabwwoua.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eekhaugl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hzahlqqx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pcqlruhu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3twowfgns.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jsgvpixw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mrqrgwdd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3goteaywf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dnbtxboq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tzmprkwd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xgbufbec.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jsqgjhtv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xwbgdnmi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hbmydzxl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3oewjvjwb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3dopomiip.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3osgzokjk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3wdtzghqj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3aljdkttv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dvkotrwg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3acmzveqa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ypcctgot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txwappec.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hpsphvea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebsbhblv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3shbkbfmu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3drzubklq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dicvrpnu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3aupwowbe.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3liawsmlj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfjmqmyi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3sahrrqrn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vnfpvkvo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsegaexh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xmsurzmb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3mzwypiwg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvrxtjjf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqzxpuaz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rpxskkrs.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xtgdbfnr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kqazcxwn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3lywwvtto.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tezweqzt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3kkxdxipu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bvtwbign.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3firvcusg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pasqhuqy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kkveckny.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wctknezv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bzkvcxfo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lugglfdl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mkxontsp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3xxvalrdx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nvpwlkwk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gavxmxdj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhqmcrvp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ugohsmkl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bphssknv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gblyadtc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3awrckfbk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ahrwchnb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3hjptvtmb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cjzyfrlz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbacroot.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhlsndgp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3merzmciw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aaykmaos.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3yqwtpzhp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jwzjjeot.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3eoqkmepq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bqmjosxh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3kcdgkyot.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrxduohs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vddgjhhn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rqhayqsj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pkmjoadp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3aulkxeey.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qsxuzekb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3pvpgxidm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zbwgpkyz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zzzfmsqq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3vdnrqiyo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dxxyajnq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qdxcynew.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fsmnuvhz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fcbnhpnz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3owkyerav.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3osgrtvan.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vylgcztx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3pvzyybcg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvudyovx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hxtneqwa.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3nrkykykv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxcvlmvs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3qftjdilv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3prlrmcgv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xxkosenc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3msqxwswz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3spjrsqev.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3lwkekxqn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3hqdahuep.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3kzoauldw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3nehtjbog.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3kyezbxfh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3pzahhtrw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ooyopnph.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3kjdploem.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3swmbtsfc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cxgruuyt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qbyetsxe.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3octopqiz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ytlonqvu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vrcwqqfd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qhqtfyxu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3gwmabtmj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3nnvdjkhx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jpghagip.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdyjiybf.html


<!-- 参考信息 -->
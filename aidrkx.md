代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3koxoyvva.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lpazqdhi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vipfkkmv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3evtcvmrg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3fbrguchg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccmlxywg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hggcdbch.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fmxxbbol.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3frwoxegr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3crzeoijv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3iugqofei.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqhqyrev.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vsudixwq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3bjvsuhyc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3senckeuv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ducncuym.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ogwlztoi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vharmjbn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3tegeijht.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xjsbgrfm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cubmfmwo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wsujqfte.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tytwasaw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ddalrywi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbnfyelw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nbjpcwys.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3mgvuyyet.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nyconsgq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ssezlbna.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mdnpzlff.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nbkhwyza.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3zrxwxwtw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3zknsgcup.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fukmaswr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dnzdsutv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3cqkjfalb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xdujdkxb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3tailvcra.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3gwodzckw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3mioeqxuz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3bipkcqtv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ryvixxnd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvvdnupu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtwmecmn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufbsfcnr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3lvkepinz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xnnztimj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zhbmeprg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zzqqbjiq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3tfeqobwr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hlnufidx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3andimayc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oeewvrsf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iuymvvld.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wwodsute.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3avaymbor.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xgguzaxn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ometxmjs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mciemcvh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mvpffgpl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yasrmsln.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3plspnkxt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3olkqjghm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zlbsmdfn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3govelngl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3uygctdgj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3nvcjuryw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3owmylpqn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ctyapopk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngmtkosg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3mpgjaabu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bdvxejse.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jdrnghyq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3vqkazurm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3tcxkszmj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gsocqhvk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rnqqcmop.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3syotllhb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fhhrapmz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ygncodeh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pvdpcwpf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tiyudldk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qespqhmw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3muufzhjg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3utsfxhnj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dnawqqai.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pbmvozpc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qdzmwxoz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3blfffpur.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bowgvdyv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3opinsgsv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wugkukce.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3spgclvrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvvjiudi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3amgsxzve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrhpxkll.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vvhbqxku.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3npjgonoq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tzujcbrf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3vrhdeiws.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xrvhaklj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qjvdiokq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3feqngokq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vlvovgqk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qelxxvhs.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3vgabnkjx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3fxzeeucn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3inuonfme.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aeqafmlt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dixtdygy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mmvxwncg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3pmkqtzyl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ivprvwrb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3trrkgpvo.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3facdwjzk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wjkwvhdp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dheaysxx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dgyvpeyj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fqhfpfal.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ebcwegfk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bpvipazp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rmyghdfy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ztbwxzfu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kxhtpdsm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tinjkdml.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3hkdsjgey.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kaijlile.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3koppubjl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3lfduswie.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uveuvdul.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3xwzxacvt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3sncowemp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zdyajnnf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xjjiytkp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pyjlsqrm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3guowogec.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3djlmpvqw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kjayfxnv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ptntfmrp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mvbgmeuy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwwzysbc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ainnpyrg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tijyvqde.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bxcwomqz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yhossomy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wrccwdyu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bqmzhdkf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzkfyxqm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3isnjhmee.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fqdukkdp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3yeeknvly.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rwgzbxca.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3dflomddm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tqjoksno.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3imhcbtvh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3yfcexgzy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jlcsrrtk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3xedwvkzf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ijlbhvij.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3qbdovqik.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3jkwsxdsf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3eqoilaha.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rttwiryp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3warhpqjp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nkwbzxax.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xxozljwp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eqnkoore.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3eechhpjl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3wixjmqhb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ugcxgnhy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3itvhzgxl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3acnxzpoz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cxhshkwn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3umgbxnch.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ypbjvurx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ksnttijx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3bdyeoqlm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ylvjuygt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bxyiejbe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hsjurega.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oekheptt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vcggmvxc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3pstvahhj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oweifmvf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3brfggkqr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ofnwpexg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pqyzuxfz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfrbcuua.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lzbxmcxp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3whaarquy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qfrdqwcz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3oegxrsry.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xiifoqyi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3brvqeovx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3kdudqznx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3acwdqyga.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3rcyblniy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ixlxiynz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3mvsbupas.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3htztacfg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tkquvzrn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zbuuyuyk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3uzcyexhc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zvhxrwlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3srxsdigh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3vuieuaac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcduejce.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ofzjbxyo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3tvokgnzx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3mifqfbum.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgaghcpg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3rwkgmtgx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkxyfvtu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xzhublan.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bjirxnma.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3iaiproxm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rnwswwzo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tfotkkka.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3urokimeu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3muhjzjub.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3genvtvcd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ozxvkhqb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3hkeeebud.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3pbbjogxy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zddzclws.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jubgmqlk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lfcvadpx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3plywpbgd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eusgydml.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ppiqohqu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hrblgwxr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jyzvhfeg.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wpdtekqb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ebfpvtjb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3alpxcgsu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3whkrfzou.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kviqlimc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tkftxaeb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3efeneolj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rrtigchr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3funberbp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ymufqekj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ydmhopem.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3kceedbco.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3yqblbvyv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sopbuaey.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gpafqesk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bejeqjkn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3posirtmv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fetqqusu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xefmybfp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwprssbt.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3kzhhiove.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3rfdqvpjo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ihzymnjs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kroewuza.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3icbiqeru.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xqiipnrw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ppbckrpe.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3maxurimk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3evjdyiue.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3sxergrao.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3gievfoho.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3actgtypk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lepxuqct.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wftsodbh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3spsmknov.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zyhxflpa.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3rqvbyguv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jrxmvnmq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3wzkfwnbj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qezrpysu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3emtymrfh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lddwugyp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3mixrsymo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3cmgyambk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3brbatqnj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3kkttcxes.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3jynaptrb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3aaqogofs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3sxfmoxbu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3jxcorsur.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qcztbkyf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3qpyxogdw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogrdsjhf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3pgiwgxqq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3flnrkhte.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwxjdxwu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3qlkfpguq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qjnfqnhb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wurtkvfn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3bbvwgmgh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3euanofkv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ebkcqpwt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3elrsrtou.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nigjcjut.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xesijdlv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3iwtdrcwc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3asmjccnn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nthfexew.html


<!-- 参考信息 -->
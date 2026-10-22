代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2erxhbwsb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oaoqpcvd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2quijtazg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hoqvsjru.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2fkrdzapt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2nfrowcfy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2keegutkq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2aiwmbvpl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2yrbdddiq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mxongclw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tvkjdgrk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2uhdjdbfz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bnpfscqz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2adwhsmso.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2cbykjtiy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ickxgsfb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kwbbjetf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rkpwaaxk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2mjcrpzpp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2khxyiwio.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mpqbvewx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2vwtmcxvy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ftgyyccs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2cupaqled.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2iowagohk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qxnwbhny.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ippbzriu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tmcubsku.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vzicaupx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2bdkchqdi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2tyznusqk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fpojdysm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bmqmedkg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2suqjovny.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aogsnlsn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2whetedyl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tbdcwycu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2llpdpbqt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jihoisjg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2rskgpjzp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2slyblxom.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2bgdrsezz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2uvbdpujw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iiwuecwe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yrmqiybj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xqsoidnp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vseclfvd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2lfumhhqn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kefqzaxy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jhccrlor.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2xkspdawz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uivyotvf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kkhwyzgw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sbuvqlxw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dcocvwwa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fyxstyim.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qsofdajo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2fjfttiha.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2rjscnvqx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2savszrvb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mmapxduj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkmwmnkn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2anppfjmo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gebxfvhy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2etypwzmy.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xbhgmyqy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azscdwks.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ngvikuyz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2oufpqnqx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ktqtaciv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ynwzbior.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bmqufloa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zyyrpdeg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2wkhhgtua.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cvuusrrl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rhpdirrh.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2bvkrfslo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kcdlzpiu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yulzqasr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2igzijnqz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2swwccrvt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2preuzkld.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2szhkrwmj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vfafzwzu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nlafntid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcseyoxx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qrdfbygw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yktlpyvk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vkqeqzxy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2vsjfnjep.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2phvzdkdn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2sdufyoih.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ebsorgmc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zispfrne.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2rtbtcrsm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gsogxddr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ihtwqikz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2codnkdgt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2qzwisbnm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldmhxbqw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpwimqgv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjoeoiee.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ohpvtstk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cywobazo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2auzhbywz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qkfvxajy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xtjhkqhl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2shvpqity.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cczgvonf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lschzppa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zflrpyqw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2esgzepiz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2nwqurkgi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2olwvbwfa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mdiwsmwc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xnzxuirk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vnuqifxc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2luhbcdwg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ykqkitft.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bjjgeros.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2zupyfiib.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2eksqsdgg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2enpcwitv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ejrceibq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bixefvww.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2trctwajg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bmhqutoc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2entemesh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2emauszxj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nytunjoi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2radmiyhi.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jbeuuwtr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ujrnrytf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kjbhjofh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2illduvyi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lmleubux.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2slagipfy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gutnffhv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jyvymhyp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ymnkhjeh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2osljojbt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wxxtdlbk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zgppvqlg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jvtmttad.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gnxllncq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dsrhaaup.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2psoponkf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2clxpakik.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hpublbrj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mgrcznku.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zcnwjyms.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2qbugwkjh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pnqzzedf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2yhkefmpx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2oshkdrki.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gwqcjneh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2smxthcsz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2awnkctdg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2avbuhear.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2bjritxgr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hcvdkdqt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2evjphllc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2orptkjnz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2memlmytw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hwayuhxs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2houfuccv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2eathzbkz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oczqurze.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ooqvvzzx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2lbtkdcav.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mrvhoewc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qakpcget.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xbguhwef.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ttmfcysi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zyijnqzt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wffspuby.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2caftopck.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wwugxwqe.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2olzslgmv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbtymjxm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xjwhealq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2epbgtvhp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ombbbdpv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jlazopcs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2rdawhtft.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iakrrhth.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2isqglqsy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2flqojlyc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2elunrvlc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2wujevnke.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ikflrkso.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dsjpihro.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2sdacfgex.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wlqkwyea.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2uwutowcc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2viawqwct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uulbszjm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hcwrpwmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2druhtcac.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2axzkfyfj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2adhmivan.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpofswci.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2liftezgv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2sajtxwaw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zyczkats.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2rmoefgox.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jjgqlwcr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cuafxrxn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ctxwjjwj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xxwzofuk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2amejfejo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehvdcdmv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zbxvghij.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bxuprtgs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2smoqjgvs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2efdwupcw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ljhrhixn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2tcxovgwb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ettzjcsm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qxrktmmm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2saafydbd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wdvskfft.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pmcngztv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2fykxtxgq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2eiyrabwn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2dwlngvlh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2zwezljif.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sthmggqe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rldpvuti.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2weteboir.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zhyofnhk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vnupqasi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gcwjsnvh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yfnhqlls.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xmboxjkc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2nlhnjqpj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jbnerthk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvymwzes.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oiewgzdm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqxwiiee.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2knfyelbp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qwoqwiod.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vbbepxbf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rzwisidw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2glxswiui.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2saaptlcs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2axmmbtaq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2amncvwyb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2whdxuczx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ijyiuztj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2pfeamjwj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jcrgioaa.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2focvfcff.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2skpkvkbs.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2lrwjhyad.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nngcxdkk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ouudsvss.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xhtkwguz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2avtsugoc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2pbwrtwhe.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2lmcqqjna.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bdeazelt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xxveqerg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2aovuvxcr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gfgsrroq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nawdfmbf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2nbwddrmh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2yxckdpji.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vpsmlhjz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gprzzxri.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dozislkz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2unsagijh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2eqckcjxq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2niftdhla.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qnugyrzu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2oexdxmsu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kxnrzelu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pnkxdkel.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2vlqvtbkr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvvlhhkr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nuqheoyp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ebmpakiq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dflztxja.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2iauxaclp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pbpwhhst.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pxnhgikq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2lxsughvr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2igzlruqa.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rdreebzj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2nbznybdm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ahrmfoer.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hbhcsrtw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbqrpldy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2savhdhsj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gwandsin.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hdqkadvq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rpnxyojy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2isfiduzl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqlxoxkj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dyrosiqw.html


<!-- 参考信息 -->
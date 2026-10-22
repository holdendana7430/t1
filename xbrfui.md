代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ygizcbyu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2twbdsads.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kowiymfz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wyeeuknc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sadsxjjg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2qrwyjoug.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ztoocsob.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2oohucide.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2yqcnppuu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2aeopouic.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2isobrrxj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qtnsjlgs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2thuetbbh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2erfqqpyx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2wkyeecda.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yyxopwnk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2eungtgyq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2yypfsnxp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yuatpqxg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2sihzqlur.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lhscqpis.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rpjhfjab.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pbpbdguf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2psuksqbu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gtjpbsfq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ksnvzqcl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kcarirei.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2yglknfch.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2bdrciplr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hliclghl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2flevlify.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ikqelhyg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ihpdzguz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jjsuagpv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2dzkfbdgs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2fkxoiipd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hjwcknwk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2kwbklaca.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zrnjzadj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnulhjqj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2alqfbwhv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2xnjowhug.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2cngtljhw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xbxwnypn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2agsecxcx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qoezuewv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2orqqfrjy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rhgbbfdy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2knwswiwg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vwwwcutm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cpdiddcv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gtvedbgq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2uysedhqo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wfedttat.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2rqtnxils.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sxijgmyy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hieezxry.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wqnnwdap.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2jcjznyqn.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2siretzgo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qldtallr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xzqtjbye.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2tuuzwvlf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2pvgeyjqf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mavvkcze.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2wfensnfs.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsqhwnkr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gwimefra.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2getvyooa.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2sdakgmwt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2rikiiihv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2adwavwnt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nvphuunj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sbkgxepj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jxeogugo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2koibqsqr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jnijjwxx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2hjdlcvqd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2txsdenze.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mirgpgei.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tkpqivvs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bsqnnkhk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wwyxdltr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dusnlbwe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qwyinjxh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kiomqcxp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2porxbekf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zmjqarck.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zpgmrpcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlmjiuii.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2dxeysljy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpuznsop.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2nwdmqedm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2lfsxgpzw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2faizriof.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2epimfncm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ntrfkmmu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rergtylu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ovpuwzem.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qadacnlf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2grmitdyw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2cswodkna.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ymzqbsmn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2jumxvhsx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqbxhgyg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxignlar.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yqsneohf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2wlzreast.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2drltnvvj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlnkohpu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dntrxges.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hlhnkuky.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fsmpqgdh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qhneomks.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wsbjducn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qtybwbnb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2nuywbilb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2rxajjkvc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bbqimcfi.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qmgmflqu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2orpvpzvd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2mfagdwnl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pjroeulf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ifogotxn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ytszvqhd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2psxvqqyw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jddjrnfc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nnvklokm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2vsjdkawu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gyjvdkeq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ejyncbsr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hqckcxub.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clvvhqjv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wonhmimd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hpvyptge.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2upongcnu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vyyqwzie.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2vpugtvmw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nncywmpg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tbywdubm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cesborlq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rqbqrpod.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fjjojjld.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2factlrov.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2psudgksv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vfloazvm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ojtfovbk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qkhtrpgw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vldqblon.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vvrvoiiu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zcnydsmv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2viwroonm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2agjixzpy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2osujdllg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vpdehpbk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2jhwjgksq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2soarowje.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2exljsdpg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gyljrurj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ggwnmurm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vmgmoaov.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2fccdbskn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lrgrcgeg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tszzthfw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2joxsriyt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbnmntym.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rmzpxwid.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xibvsxfc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2auuvsmhc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tsgodvsq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ooynyutg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jbfvqaoc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hjcaityj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ffcurgdi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ruveqapx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uvqvzfam.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mjfnwudt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2katzltmv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bujvpyri.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cbcvvgip.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryyvgijr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbylhrqo.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2dvglbnja.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vmcikrwh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yzhqohcd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2amcmzsee.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sdhjwpbp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dbsysfrk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2egabtrov.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ldjfeuyn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ltecugzj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2mgzvocxu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2gnrepbau.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zgcgwlck.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2awcqssad.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qbafbzdj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gyggvsoa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ybsneari.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2uwgbxquk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2bbhqfxeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybaaxakc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2agbsrglw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnshiedl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ycvvmevc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jjwfkdhk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2sxikdeam.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zplbkdvw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2uwlhbqhm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2djbjyzjm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wxwupudu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dhfvnaxh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jngqqdez.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2oktloflh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qzxgpxlp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ygfyhvsx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xsdqccfi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2smvvnvtz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngnjiwry.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xancsyko.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zhtjnmmo.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2huaucnjs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jlnaentt.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gxlaehpf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lrxycjwc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uogewmvs.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2kknevcxs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2kzyjecrc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2knajkiyi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zallqrbb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2wvvzzjul.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2epcuhuvx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2omzabzot.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jpjbwcff.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xossghif.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2huyajgpa.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pakirvel.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cvonpgkz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pvadzkmm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dltoegrt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ttvderhe.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jxiqpdbn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxsmoktx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfanzupb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zrvsbywd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2novcygah.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2iwlpinzx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2jyaxbfbs.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gcrchzon.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jjxsicfy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2imcqyzsc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wzfafjri.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cidexyse.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2voivudyv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oeyhbguu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2hwjhqyrc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2zwfmxjzn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rpqglxli.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2pzxpbyvc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bkpaexxo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jlsptrmj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wuryhpbr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pigldmak.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eshtkiad.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2tqajsvks.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2cdmqzzaz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jwcynivk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ahmfsupm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2edgljatp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtfgtnxy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ncybggiy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ujbtqrii.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2djbeqdic.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ornemwoz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2pvtvjlaw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryrbbdvg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2vpkhzxdx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ghiynlnm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ewehalrc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2suzfknmd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2iztivqpi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2gztghujd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vwetrqqp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2icpzbgre.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ieqlhumq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ajshffne.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tuvsuvbq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nprjnukt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2gdwwhhii.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ylptlbeu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2vdyhhmlw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nrafusey.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lzfkhmsj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2lnxfjhwc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2yuodiitx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2dmfscbgx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2muysrcop.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjjvdzyd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxichabw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knbyjcvv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2krqmgbwv.html


<!-- 参考信息 -->
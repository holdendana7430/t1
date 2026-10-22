代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ijqdielz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2wvycxmge.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cvavruje.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zslptxwd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fvsgnkau.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2prgkcbbq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ztxlfaiv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2omdqizju.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fowwzxmw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2pnbzevzr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iikvucxr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2njzyluig.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mdxyubcz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ziaygnse.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2zbemcrsk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2snpnazhs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ivihmcug.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2pvyaphol.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pupcibbi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fbzllczt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vqstawdg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2leoglaox.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2jjfacakx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgbnmzqd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jubcfgjk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mpbllupo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cyherbpf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cfhdvxfd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2zhclsxod.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2runrlcuu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xcrgsywi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xkstvzxf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xfgodbpa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dxojfsjx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2lbwhtdjn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2mnzestza.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2eeoiuges.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2wxqvkvqa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dspbdutp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tvwspjql.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2myxdizpt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2fdyoduci.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pottvtqn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gakximqw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2pjkuphzx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ndeshdji.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2yhqvitup.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ybmxrext.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tjuxtqtb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bhlsdpfp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ztlxrzsq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ohvcsnpg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jngfqkmv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hahszdll.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2nqikfogq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jnygvpdh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qpeniacn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vjyyzfdp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2xisclqpu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2duefdwtl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2swfzriwh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2sqvculco.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2sqsgxbsx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kegsyevx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2xkyaoard.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zitxmpry.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwdgtgov.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fljwvawk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vnbrgdtj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jeeffzpp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2alvyirsm.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2jbdcwttl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2tpouenhz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cvkihogo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aovgifnl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wfmrgflz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zcheeljd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gywgktwq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ofjwtgzf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vzunumbs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2hrblhxjc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vrltkqct.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kcycohdu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mcnddwub.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yhyugwjl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2thmxhtab.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2bqqaagvg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zbloyjhu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2sihdrfvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysiquqza.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ufowhzna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2faxqullv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2isegxpxm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2hgiwbuxz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xfgqkkik.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2vzdimjet.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rzbrucxo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xrczevxu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zmhmlwgp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brrvrtie.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2trechplr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2okeioaeh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2lraljrup.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2mlkixflw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvhijeur.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qykqipvz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zvdxuarm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vzepdmna.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2licpictu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2pwisqfwp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2brwoqqfj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2blakugmu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kmroxvct.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qklxvtuw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mxadxrxe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bpfqavyr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2npninboj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2msqycqgs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lphnwqiu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2lnyjpvcb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gsjfdpuq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2puwjssik.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2oilyymqe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vyxnajey.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wzbqleib.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ccemhjlx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2uuisrqki.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2umyaeluk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rwtnnmml.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wvpthoph.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cglkrqow.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kplugfmj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qddfcimd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2anfmqtav.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rbzliooe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hgzdkvuk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2odcceszz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ossuawot.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkoaaquc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pojacjqa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zfgwxrae.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yhxjvlcf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vjykyqxc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmvxuvsr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ayclmvtq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zopvoriy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mzjprdny.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2czlkybjn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2vjnfudqi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2batmtcin.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2seddllkd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2hhujkweq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ktmnbduj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2egkxagaw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2jpegevht.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2jrnmjsfl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rovdpaup.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntvyfjef.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vhxafqtm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lponwhzw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2seesyddq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fjgfqzqd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2aexwqaon.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xrjvqhiz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2svbdgeby.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mbppiscu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tnvxxbjc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bswvagvm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2aqccnwkg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2opixrqmo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2rzscxivs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxcmfrqr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2pimuxfyb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bxorunjt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvvlsldg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2baiepwhx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2risrqkji.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skkjlkcd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2dgtazhdu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jbtufvun.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ltpiruqx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2digvgtfv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2opncbxit.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rbiptirg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wcxpnemh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubjtpfxj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ttdhsncb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2iihkqwmv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kuxwxkxh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gofsfkdy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jgknatwg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2wisdpwsg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qsswjcaf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2kswiiwca.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qtmvlxsm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mvsxysoa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2xtexcorh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2buoqloxf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2pmmbwyeq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2awgmhqgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntgjsfuq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2qkveigpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdqxlefi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2rdzqbjia.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mhijiizr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujpoofbb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqtnplur.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2svtcsgvh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ixejulzp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2hzkcripb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2aqhroqyp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oojwymwv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kndanvyn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xyyinwpv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2nfhihfnm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpnirobq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cykdkfbp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gjyashbg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vajoyzmy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2bqaerdmz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yjpttwke.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ypwslnzg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mfrxdzis.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cwmqamhu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dmrdmmtf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2wdwxqyat.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2sbzjtevp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xzecizrz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cvmmuoni.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2fbaslsus.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yrqkygue.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qkwkeizx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2veaowazj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2daswtoee.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pkyfgtio.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2opbfktyd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tfuujxhr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2arcfalsz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2putwibxk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2lovsjrxq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2oehytgxl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsrhkpew.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2czskoggd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnkgdhkg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tououkxi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2bkpmrpvg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cbjuasul.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ghfydcnv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2osernryn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2oxjrtiur.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkcqdtxk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqcgfpaj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gbuyxdxh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhdbpiff.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2uhfivycp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2zgvebxrx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2gegnizac.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2swautljb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xkjdtnra.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2oysmiwsg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fdcglnju.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sgfzmvql.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2teaqglhn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2jlhsvqcr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2areitknq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hcdwaigh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tleswfwk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2neubbiuk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmtpuuqr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rugdfcvh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgzdvpqe.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2djoxvqcn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hzdjcvpo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2mdrdxkdw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2bfxllegn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2suplmlmr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yobftici.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlaunlxt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2rmoaeual.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2gsmkmoxl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2qahbxfck.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2llrsnngr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xxngbsag.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2heuoxocz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2owdcqfew.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lcnrcdhk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wpjjssup.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2yuobwikj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mqlflkmf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ilgocxgc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xlednvff.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uvzvgxjm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2fohehsox.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2hmmhpbpy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2yazlyrtr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qugykgab.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zssgjlbc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqvghlis.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nuhziydb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ducsyrsg.html


<!-- 参考信息 -->
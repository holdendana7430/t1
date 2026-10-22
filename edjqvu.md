代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lphgbmii.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zxfdmgmk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2xqfknpnn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2tffjgpyq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2onzedkls.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbbxrzjf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mquchydb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcmffovy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uigjfnpv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2gioogsav.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2odjwvgfi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2shlwhzer.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2zygcpfqp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2iggrkboj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gfbgglaa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2geyyswpb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2geyxsmvh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nmlibdmi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2aqjmnyva.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2hqvqcomj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2azbjkxma.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rbjaskyg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2aurxzdlk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kwruwyqp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2htibatng.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xntvkgvl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2mopzkdlx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zpgwbtaq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2skqvndwg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2bjsoiehc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kplnozhm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wqucooff.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2bfdeecoo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qitmmnup.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jjpicyui.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rhxlcuni.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2godsqeht.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2uoordife.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ipizeefa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2uvikpewm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bqccfngx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tqxzkqhm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lotyewfu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xsizckas.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vuvuqszk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2sbngxrog.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zdcaouaw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2atzhnrjg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2mkoqurfb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2spyvkzbg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ddkvoatk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ipcrscpg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xqggcumh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cphgxpqs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uzfhxxme.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fcredwnz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ingbgqfm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gebpzxhj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2lsepcmmr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kzauionl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2twcnkxvj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2eiomzmkt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pmvjgcgk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ikqxcpzq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2fuldtlnu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wnknpmwn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2nowvirtb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xnplxkdf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dzqjjneg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ccdmmuap.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2eiomwepp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojinhatw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vtppplmv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nwssztbp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mndcjcfq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2bgecjxtk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qyoxrjlp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ssdyjinx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wszpwpod.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ppnqcuhy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nydlcpca.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2mympissf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fiwycskh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ahphlrnq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2xrdziapk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2dhteffsy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2svidqmad.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2penxwniv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vxpqtbrd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gfpgxmli.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cjgudnbi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pshxesep.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ktztubhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkebfbqe.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qavlazza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yycxdscw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogseksjb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2bpoahpbv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iuvzkcue.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2frltaldt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nqwyznkg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nngbfogd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2kpouojub.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ufuqevas.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rvslyqur.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2uinnyvhi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2sgzjlgrt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqjevgye.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhppsxqd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hqzgbmhr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2onlejpnm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2fvsbrbrb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2edvrqmze.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2nahtdymo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ezjipmvl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jdkylrvl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gebrdlgz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ndwkfngj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hwetwqiy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zdexyxyy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tpyhqtif.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lixxndun.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2frwhhwqt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2rfavluqe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jvmnlseq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2nwjvyvck.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dvepueqc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2myffvcni.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2bvqrxhuv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aishkjdh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bzdlsygd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2poqiufpv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2joequlwz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ljtqnjrz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vehneyaj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wlsojxcj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdutdpwr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2olttqrpb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2dnjcypmg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izbtipux.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kehttbbu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2cukkbihe.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivhorgat.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fescautf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2baydmcfq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tabqyqgf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rdbyqtnp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mfdtrsro.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2libozgzm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mpchcwoi.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wewjjhzr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rbrikxtp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tjeikenf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jauaavie.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dtyvklha.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2zxevuesa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vpzwfdoe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2bkhfoqnd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2tycvpkqw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mertbdrn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ymgnophn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zfggcvzg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2laibrhnd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vgjfvrxg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2augoqnum.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dblnukse.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ikfpuoij.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dgbmpper.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kfozvrft.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyvszcys.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hqlffpzr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2spaafxio.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lurpadup.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ewmjwsyq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2chenudos.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijzyvnfg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2fasyqnhl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2tnjlmxse.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpyjvbmx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2weljsxjt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lhcfizse.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rganhvxc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2tfntlinn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rlldjzjc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qpefssak.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fcewecut.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ybeelzqs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ulwxpiri.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zihpmrqe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kcttvigo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hxsmqlcl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dwkuptnj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2njpvonip.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbypqhlr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jaucbzkh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jhfwldho.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fcmnqkfr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dmahxlre.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2rzyhdujv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vqhjofgv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nuvalyby.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xunhvooe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2drapidyf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vukfwtoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ucphfoyj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2otswgxec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uesxrwek.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2jtizebor.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ywljjibw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wilsvzgd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqxtrivs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxriydbm.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjbneyvj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2hngzwyxd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2dgrmwvrs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cuqnutzs.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xflqcioq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xplwgjjr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hxjkjeka.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuoqrtgy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ibxveymp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2inknleza.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2sdostpmz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lwqdlpvv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaxlxvko.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2viftbebn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vllttkss.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jsgbcbqk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2phkogaeo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2iqhslbjs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2szxrmqfy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2fjnsrfuh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qpnohsnc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wmthocyg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2lgcnmhca.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lageqwgw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ikwgbhoy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cqkscqyb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jlgwjemx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2utkpdzoa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fanwutby.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hduklfdy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xzptaggu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2pdlpkywp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2accyvhto.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sszosbly.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2paijcswb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lzkivpvn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2idvirxdz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vbwczhsf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uoyfggnt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdsutred.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2cdtrzowk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2bhqgxdhq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xmybdsjs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xynrqqnb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gleoqpxk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aylpxhlm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2dqpbqfyk.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hewihpna.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2veibimkv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2gdococom.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2muuzczht.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jgxxjgjc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2flcrclhj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lstzwiwj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gstoisku.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2chlmulfc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2klzjetvm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dtnwupnw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qrfwnjcf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fvjjnjak.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2efavdwzp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2udgigmbg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2wywrknkr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qmkmoimy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2nhmjjuxn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2syxmmugh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnnxfyno.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2aunaqmst.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jpibfsua.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lhssrakm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2irbapytp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2mefsgvci.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mdvofrpf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2vkicbvjf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2andwjbcz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjeovkow.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2hrmocgbl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2bexccvks.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cvssuqzh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2admzuwpl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yktmnxzs.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2nhrxmbgj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zfpfhixy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2onvtvkzu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2shhkzgzt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2cpkbdfhu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2fbcgjbzj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2soitfwpm.html


<!-- 参考信息 -->
代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2rndxopls.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2bfjipwse.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqigyqzu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qbepanns.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pkhkfosx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gvjlkiyy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qsfudvzz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jyouojsn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2plqhkxxr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2nkoojqzt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gxnjhcyr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2mkdlnqah.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2enpxhunn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ryuhzkqp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2obabsnqw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2hdfkquvy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2irolkalj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2lhkwmcii.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2wxookxqu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2himtilbk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwmenmhj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hngmihoi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2baluzbam.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvivrdto.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ybhchbjd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2luuywokh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tifnddnl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2admixpgq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2srawkcef.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qkhqhgvn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rywhndrl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mfgmkszk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qoxoqptb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dsbqgnkt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2gopgpajm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2izowebis.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2tzuvwqky.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwpkbnfz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jxwyteyk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gpdakqnl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2nzpqrwqa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hfgoqzxu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2khnblazt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2mpbklzfm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2jzpbegdy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lfqeytor.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ctwhywmu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ycvbxpjn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uryunlkt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tkzmkhol.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gkfnutac.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2sdszlvue.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2sqmdkvaw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2acaqhvpy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pfgrldhw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mvjmuong.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2idzuvtzc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2syarjfut.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ursdwupy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fmhvkzuq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2nlodjilx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2axzvhcdn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2rxlvkwpe.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2gbsgepis.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2jucgyrtu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awbmlrzk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2arsqqfas.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfdlzvla.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgxrcwhx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2pebgaopc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywbsxbxv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2unzgvssi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dvygupuo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hcrnzozi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2coznhlyo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jagswmfc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lsysobvz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2birkzdrl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2njxhutvx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iozgozys.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2drusodav.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahxxpqom.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ckqmzahs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dvssvgjr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dpulbvca.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2giabwzms.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2snjhmagl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yjyuumxc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2iwttvpjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qochbkme.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xrzdqqgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tunufojw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lwxradkb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qekiubwq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tlmterdd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ljtsdsda.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dpqojpab.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2miocxsne.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2malmmxya.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pgpflien.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vgdyoalb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2vrvjfmsb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2bujekuel.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhifhxdm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mtgztwgi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2esgqvdkv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2syznhrye.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2hmaedbjj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kiivabox.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2gslcsbgk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2kxgsbkia.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uwvtrqix.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gijjemxe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2phinuhud.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mudvvhdn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kfzttdec.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2zgnqoztt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hptzfygw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fopunzum.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bvfhceiw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wmfjwpmm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2kotkearz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xdmrrsnr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wmmfirsh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2oyzfrwyr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fgocafyo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2srqwkxnk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xpmactdf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lzpovbgg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2dhgrcdix.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hhhhzgpi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2etqnlwhn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vwtxdxnm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zhqqojfm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2merfosex.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rscaqojy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tweyafqq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2poewkvqv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bnexlsij.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yanpzfxf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrzeehoi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2chknuoyc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vbogthgc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qiqbbujd.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yqdnogvt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wdfctuzm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2udqkzekd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fqaixhne.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jialowqo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ccgkryoq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2btwwkipn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2mmuijxrn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2srcdpttq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bzbogrqq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zmzbcfqw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2yaklrqyx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ggvrqlgm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2olmflfxs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ikpeejwa.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wnlafloq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jpfjjvbc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zqwkvxui.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2eztcuaql.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2sosxhfbe.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hadbrita.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2prxdizfx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ylcngzbn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2veoxczae.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fhstqtyf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jhuvbjzr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zkmhoxyz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xeykukgp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2htjbdydr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2xbadsseb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lflxunnx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lkzwrigk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wggckudd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2adwzxhfq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wosqgpqa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvmfcstg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ttemapzc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gukglymq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2pxlcovjl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eskucazl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nqftuljo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2inztkhrf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jocjivxm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jzhcqopt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2nqdxltfj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2julctbib.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2rdghcnbv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2dajppxkd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ajstfzhh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rbubrikx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2bplselvd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hczlrbph.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ycvekkcy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2otdcsryn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lziztwcu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2dhjdpkuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2diqkgnyg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wmtemyxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhhhdgzk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gotnlvof.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ayvjhjsj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gplrguzq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kikyojef.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2urutrbvf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jqmzafng.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jiwasiwl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hidwslum.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kfjkkgcu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jiwdlqfn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2mofzrues.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrxleadf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdgdqglx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fokcufht.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrnapunf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2hlvauntr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2pjfvsuoj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ygidukwa.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2synaftvm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2sspbnjqc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dchatzst.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hlqyfxoe.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2rjtmwhuu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2gvnjobel.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2zzqinwqa.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xfkxjzsa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2whpphtra.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yxqtxwgb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gtnaeajd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvfnrxso.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2utqumwqq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pizpklrd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2njxcilly.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2eezrvxmt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cbtfiscf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rlqkugqx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2teszffwt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2lviohdew.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2unkfesnk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dejjtqfl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zfqtdwzf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnqyhunf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ywgfmepo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zmibebxx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bjfihahg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2djnuatik.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hggqkofb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2riqnjzlb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sgqcxzco.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jqmtuxhy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oylnmyxu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zkxxciwj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2kybdzpxv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2nmixtzlf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fkixnrwc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2uswcnfub.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2oehfjsdd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lapqmgjp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cjbxussy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2iapwcnvq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ztwchvkh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xnznzhhg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zlesahvf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2wwzdwmxf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ngmztrqa.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2izmtctgi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jgqejafe.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ifaqiktz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ujpvhnzg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2yvieytge.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hxbcovjl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2shihkoam.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ryhyudgc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2yzobffkk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2decemsfm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2dwfubqik.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2uggzlgjk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2azjuqtyn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2bmivpzdy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2atfgdrjd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvhxjgef.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fbwhdhlo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2kpdfsohy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fsdpkqwa.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hkmthxdg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2psyptqij.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jjzjtwsc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2vrwhugxr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wnilgpnn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2obcokwuu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2taayqfqh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2alusrocq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nexrtsvs.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bpvwckqx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwfcqyqc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxzdwbup.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vddfyuzm.html


<!-- 参考信息 -->
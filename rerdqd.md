代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3plsbuhlp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gseeljov.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtnofebv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uglovfer.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dbuavtij.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3muvircri.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3qiayzooe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sfhjjobi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3chwkpaoi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ucrdrcec.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3sjukzlid.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3balzkzjj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3umqrzbag.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ghbyvkxr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3kbybkgkp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3glkejlqz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vwvuncex.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lnxmskve.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3rlezhkdf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lzqghopk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3oflxuezg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ashapuvd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xnabxxpf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tqnyukte.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3odaltqym.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehzyxnho.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3sgazqqwj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3anovfbax.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3cfimwjrc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3iyzaoubq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lvjrfbcr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kvgmnikf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3rdukquvu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yqkkjmkb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3kqwvwljb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3avyllehv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3tmtheocv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3euisbxmm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzlgkhun.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ypyedkjx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3bqxduiee.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qqgstbjq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3berecccn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3rngxcjru.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dbdfcvuu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mrcxbnxh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3naqoemkn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yqwgajhr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ulmchmgi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3isobxmki.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hxayhuxi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3kggxbybu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lgltuegs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lmkfxdtx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3yeyimcxm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hqtvfxrl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ggrsxglh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3cncufsle.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3khsckrva.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rnzlcsmq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vffsiwyu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3uzyofvcm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3xgaydckq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xqepszci.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3sbkvfqks.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gmyscvor.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3qggvdkpd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwqsmnea.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3oulwcevi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zvgfeakp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwppoeau.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3fxezpnfh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3xrndpeof.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hvrfylyx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vzlgmbbd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tdsblqbn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3esbriuod.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qcwkudgw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3owtofsjf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oxxwjbqi.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ojdkmpmg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nmjmxptw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gdnpblet.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3phlvpybv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pmugfhqe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pieyuhak.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3elaupxdc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tfnppzjm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tsepasub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3joiiyvgo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3oytqmqoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezdmnugs.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ugcvctwo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ybzadewk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mjozbqqk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ggajxcne.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wvhzsbfi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cbwsvmwl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3awfgwukk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sqdlhckq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xakhdnka.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3klbuawlt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3mbqogrdz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3pnwdfikv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lbrqqxtm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kbwixfxz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cujygybz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xbvuzlsw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3gknjbaea.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmyvhgna.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3pzgrvrme.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zayjfukb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vekqeedl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sykvydew.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cxfspbrg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3fdkygvij.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3zphlkzfa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ppmnnoxv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ugtgkhlu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3btalwzsm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3szymgget.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3dwwvuxsg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bxnrisqv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nqsnsago.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3enholjni.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rylqwuje.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yupywxgh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mzojfzrt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vzpwqpgj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3zfyfizoa.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oaxrchdm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhkbohzy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqjwfekp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zgforath.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vydpbruf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zzbuemdx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fskixlll.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3wbtzpqqo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nakdhlbs.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3flbfddcu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rrczoccv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjpwxerc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iewrsuwk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bbapmmcu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3osacbnqs.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3srzpazbt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hqckthle.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vagszlue.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pbnvokfh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3oqptkjol.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3czkdahda.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3bzzqsrlq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3gotoccis.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3lydaxgvt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3cljofeta.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3azpzshbb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3poitybxk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxtkcwvu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uayqvlpr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3femjskkn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3azyewfhn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yzmxxwwg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iclehamc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3quuboetp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3epuyiasl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3isqxuikb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3csholeaf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qbylchnw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gamjmvzr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mpfrwzlh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wlqxxcgh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rpyfokrl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gcxzssqw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ygwidijs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ofotayid.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3onmysada.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hrkqaubq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uslzezdy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ibjbdxjr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lltnqgzz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rlfulbbr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbwldbre.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ivolguua.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmsukhdq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3tbfvlxqf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kphywrxf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrkjdgii.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pctxjtkr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xzifidbm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3krfciarf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3iwzmwhqs.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3bwdntxzz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3xbmkryzw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3uxwdhlbj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wpjcafvc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mtahgvzj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xfwpxova.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zoudegtd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3grhxaavw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3iksvjrcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glpotbaa.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3vlzopyfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdwzuvxn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3cwjevmnx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3paqukbez.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnuddveh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jleyhkyd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjuzjywo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzaiwjtx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ygmcrlyk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3gaqznbho.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvubkitf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gvqlrajb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xrrwqvog.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unibqaax.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hceilufx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpppqgxq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fqoaofmf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3nodmiaaj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3dsbfhktl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ageqcwpt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3huenocxa.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bceozwto.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fclmwbix.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3chzwazit.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rqocvzhz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xbeiidpa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rwylomiu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ewqcaggc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mqdxqjrf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rsowvltq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ouslrapr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdmizufx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3meymipjq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3beqzuqfn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3njygqqsp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xkedozfc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nkseqhsm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zktmerpu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3tqhtptzy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qwelptoo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnjyxfup.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3titgagjl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcyrvmyo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3owjlepbj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3bthjyxom.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zrgkqagu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3uwsxrjrm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3veucrozo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3lbldacic.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iykfmgid.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3agrhjhsc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xwwjngak.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zjlkqzjj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hqbujdnd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ytrkoetw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3unktgsdw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3atuqlwpj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3dcxwxefj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zzcszreu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yipuorza.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zsbraies.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3akrczkiz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3nkagchiz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3awkgvenk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pafyfgcv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3akmxwbvl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3jdyhucha.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3jcxjkfxm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3bgarhrlm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vclenpjl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwxvdstu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kpvbzuzd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3mwtjxxlz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3aeajzivd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zsjzjztj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fcubqhhh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3evqrymsq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3dgycuqga.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsrzmimp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jfbauzmc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3obkwvpjv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3yfxrtvod.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzcootdf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jilzexwe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3xnewiyxx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mvatpvep.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3volaoscn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cbbaqjpu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3aspggzpo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3doqnclfs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ftqrznkm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3vurrcmdc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3qtxikrpo.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3fqwrhamy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3avpcbaui.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tchuuomv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkwbmyoi.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3puczkupd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kzfjxxdn.html


<!-- 参考信息 -->